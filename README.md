<h1 align="center">TIC-TAC-TOE-GAME</h1>


## :rocket: Knowledges
 - `ReactJS`
 - `Framer Motion`

## :book: How to use
To clone and run this application, you'll need [Git](https://git-scm.com/downloads) and [ReactJS](https://react.dev/) installed on your computer. From your command line:

```
# Clone this repository
$ git clone https://github.com/ucfx/TIC-TAC-TOE-GAME.git

# Go into the repository
$ cd TIC-TAC-TOE-GAME

# Install dependencies
$ npm install

# Run the app
$ npm start
```
## :link: Demo
  - <a target="_blank" href="https://ucfx.github.io/TIC-TAC-TOE-GAME/"> Click Here </a> to see and play by yourself a demo of the game.

## :mailbox: Contact
  - <a target="_blank" href="mailto:ucefhammadi@gmail.com">E-mail</a>
-----------------

Rakenduse käivitamine Dockeris.

  Esimese asjana on vaja oma tic-tac mängu kausta teha Dockerfile kuhu sisse saab lisada commande millega hakkab docker imagi't ehitama.
  Peale Dockerfile sisu täitmist peab CMD's runima commandi docker image build -t <image_name>:<tag> <path>, selle peale builidb ta image.
  Kui image on builditud siis on vaja see pushida DockerHub'i oma repositorisse. Selle jaoks on vaja teha repository, minna tagasi CMD ja
  kasutada commandi docker login, peale sisse logimist on vaja image ära tag'ida commandiga docker image tag react-example-image <username>/react-example-image.
  Kui image on tag'itud siis peab selle pushima DockerHub repositorisse commandiga docker push <username>/react-example-image.
  Edasi peame tegema imagi'st containeri, seda saab teha järgneva commandiga docker run -dp 8000:3000 --name react-example-container react-example-image:latest
  kui see command on käivitatud siis saab proovida kas container runib commandiga docker ps. Kui container runib siis võib proovida sinna netist sisenega url'iga http://localhost:8000.

Probleeme esines alguses Dockeri käima saamisega, kuni etapini, et image buildida töötas kõik kui tahtsin imagiät tagida ja pushida siis Dockerhub lakkas töötamast, arvuti restart aitas.
Rohkemate probleemidega kokku ei puutunud pigem on lihtsalt jälle uus teema ja võtab natuke aega kohanemiseks.