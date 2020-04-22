# Docker CMD

---
---
### build Dockerfile
`build` (make sure "." at the end of cmd)

     docker build -t [repositry_name:tag_name] .
     
---   
### check list
`image list`

     docker images
     
---       
`container list`

     docker ps
     
---   
`container list detail`

     docker ps -a
     
---   
### run image
`run`     
     
    docker run -it [ docker_image_ID ]
---
`8080 port set run`

ie) docker run -p (access port):(docker port expose)  
     
     docker run -p 8080:8080 [ docker_image_ID ]
---
`access sh`     
     
     docker run -it --entrypoint /bin/sh [ docker_image_ID ]
---  
   
### stop container 
`stop`

    docker stop [ docker_image_ID ]

### delete container 
`image force delete`

    docker image rm -f [ docker_image_ID ]
---
`delete all images`

    docker system prune -a 
---
### change image name
`change`

    docker tag [ docker_image_ID ] [ new_REPOSITORY_name:new_TAG_name ]
    docker tag [ old_REPOSITORY_name:old_TAG_name ] [ new_REPOSITORY_name:new_TAG_name ]
---
`delete all images`

    docker system prune -a 
---
reference sample https://markdown-it.github.io/  (thanks to github )