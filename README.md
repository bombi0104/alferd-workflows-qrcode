# alferd-workflows-qrcode

## Create new workflow

## Add triggers hotkey

## Add action run script

## Input bellow script

    /usr/local/bin/node main.js "$1"
    qlmanage -t -f 4 "/Users/anhtai/Desktop/qr-temp.svg"
    
## Open work-flows folder, init node module project

    npm init
    yarn add qrcode
    
## Add main.js file and source

    var QRCode = require('qrcode');

    QRCode.toFile('/Users/anhtai/Desktop/qr-temp.svg', process.argv[2], function(err) {
      if (err) throw err;
      console.log('done');
    });
