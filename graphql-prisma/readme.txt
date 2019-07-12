################################################################################
For running the container
################################################################################

cd prisma
dockerd
docker-compose up -d

Access prisma GraphQL playground at localhost:4466

################################################################################
To update the prisma for latest schema
################################################################################

prisma deploy

################################################################################
To run custom node server
################################################################################

cd ..
npm start

Access its GraphQL playground at localhost:4000

################################################################################
To kill a container
################################################################################

get container id from
docker ps
then 
docker kill (the obtained container id)

################################################################################
use sudo with docker commands if the right permissions are not set up
################################################################################

################################################################################
To get logs docker logs -f (container id) 
################################################################################

################################################################################
To access playgrounds with auth
################################################################################

prisma token to get a token
in prisma playgrounds add http header
{
    "Authorization":"Bearer {token}"
}

################################################################################