# Docker CMD

---
---
### Dockerfile build
`build` (make sure "." at the end of cmd)

     docker build -t [repositry_name : tag_name] .
     
---   
### list check
`image list`

     docker images
     
---       
`container list`

     docker ps
     
---   
`container list detail`

     docker ps -a
     
---   
### image run
`run`     
     
    docker run -it [ docker_image_ID ]
---
`8080 port set run`     
     
     docker run -p 8080:8080 [ docker_image_ID ]
---
`access sh`     
     
     docker run -it --entrypoint /bin/sh [ docker_image_ID ]
---  
   
### container stop
`stop`

    docker stop [ docker_image_ID ]

### container delete
`image force delete`

    docker image rm -f [ docker_image_ID ]
---
`delete all images`

    docker system prune -a 
---
reference sample https://markdown-it.github.io/  (thanks to github )