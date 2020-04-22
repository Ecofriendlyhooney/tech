# Docker 
## Docker
### Dockerfile build

`build` (make sure "." at the end of cmd)

     docker build -t [repositry_name : tag_name] .
     
---     

### Docker Image run

`run`     
     
     docker run -it [ docker_image_ID ]
---
`8080 port set run`     
     
     docker run -p 8080:8080 [ docker_image_ID ]
---
`access sh`     
     
     docker run -it --entrypoint /bin/sh [ docker_image_ID ]
---  
   
### Dockerfile Delete
> docker run -it [ docker_image_ID ]
     - run 

> docker run -it [ docker_image_ID ]
     - run 
   
`df`   
   
::: warning

*here be dragons*

:::


---
reference sample https://markdown-it.github.io/  (thanks to github )