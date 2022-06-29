# How to install Node JS

- Open terminal

$ sudo apt install nodejs

- Verify $ node -v

- Install package manager $ sudo apt install npm

- verify $ npm -v

All done!

### Okayyyy there's a problem with the above procedure?! 

Jeez let's start over.

So i'm starting my first ever react app and I needed to install node js...
I saw alot of new things like .json files and file arrangements all....

So here's what i did

I first went over the above procedures to install nodejs but I tried running npm start I kept having an error

``` vanessa@vanessa-Latitude-E7450:~/Desktop/React$ npm start
npm ERR! code ENOENT
npm ERR! syscall open
npm ERR! path /home/vanessa/Desktop/React/package.json
npm ERR! errno -2
npm ERR! enoent ENOENT: no such file or directory, open '/home/vanessa/Desktop/React/package.json'
npm ERR! enoent This is related to npm not being able to find a file.
npm ERR! enoent 

npm ERR! A complete log of this run can be found in:
npm ERR!     /home/vanessa/.npm/_logs/2022-06-29T13_04_13_726Z-debug.log ```

I'm seeing something about .json file and the tutorial I was following also had a package.json and package-lock.json i had to research how to create those! 

1. https://docs.npmjs.com/creating-a-package-json-file/
2. https://stackoverflow.com/questions/46653833/            is-there-a-way-to-force-npm-to-generate-package-lock-json

I'm still not sure if that would have been created automatically if my npm start had worked so anyway I created those myself. 

still getting an error

``` vanessa@vanessa-Latitude-E7450:~/Desktop/React$ npm start
npm ERR! missing script: start

npm ERR! A complete log of this run can be found in:
npm ERR!     /home/vanessa/.npm/_logs/2022-06-29T13_10_22_998Z-debug.log
vanessa@vanessa-Latitude-E7450:~/Desktop/React$ npm start
npm ERR! missing script: start

npm ERR! A complete log of this run can be found in:
npm ERR!     /home/vanessa/.npm/_logs/2022-06-29T13_12_58_779Z-debug.log ```

Now i'm super confused but I think it's saying my npm version is outdated. so I went ahead to to update it using nvm(node version manager)

Let's go over the steps

$ sudo apt install curl 

$ curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash

$ source ~/.profile

$ nvm install node 

$ nvm install 16.15.1  (whatever version you tryna get)

okay let me go try the npm start again I guess

npm start did not work apparently I needed to create react app first (SMH)

$  npx create-react-app my-react-app

okay that works, let's try organizing files and running npm start again.

npm start only worked when i opened the folder! smh
