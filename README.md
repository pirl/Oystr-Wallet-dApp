# Oystr Wallet dApp

Official Wallet dApp for Pirl, Used within the electron wallet (Oystr)

## Development

Start a `pirl` node and the app using meteor and open http://localhost:3000 in your browser:

    $ pirl --rpccorsdomain "http://localhost:3000" --rpc --unlock <your account>

Starting the wallet dapp using [Meteor](https://meteor.com/install)

    $ cd Oystr-Wallet-dApp/app
    $ meteor

Go to http://localhost:3000

## Deployment

To create a build version of your app run:
    
    // install meteor-build-client
    $ npm install -g meteor-build-client

    // bundle dapp
    $ cd Oystr-Wallet-dApp/app
    $ meteor-build-client ../build --path ""

This will generate the files in the `../build` folder. Double click the index.html to start the app.
To make routing work properly you need to build it using:

    $ meteor-build-client ../build

And start a local server which points with its document root into the `../build` folder,
so that you can open the app using `http://localhost:80/`


## Contribution 

Being a open source project built for and ran by the pirl community contributions are welcome and encouraged,
to contribute simply make a pull request and assign it to one of the core team and it will be reviewed as soon as we have the bandwith to do so.


## Gas usage statistics

- Deploy original wallet: 1 230 162
- Deploy wallet stub: 184 280
- Simple Wallet transaction: 64 280
- Multisig Wallet transaction below daily limit: 79 280
- Multisig Wallet transaction above daily limit: 171 096
- 1 Multisig confirmation: 48 363

