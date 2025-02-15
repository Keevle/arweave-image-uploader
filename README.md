# Arweave NFT Metadata Uploaded

This package can be used to create metadata files on the Arweave network. It first uploads NFT image and then creates a metadata JSON file for this NFT using this image and default fields from file `uploader.js`.
It is created with an idea to be used with Solana blockchain and uses [Metaplex NFT Standard](https://docs.metaplex.com/nft-standard) but it isn't bound to Solana in any case and can be used with any other blockchain as well.

## Use

Prerequisites:

- all images need to be in PNG format
- all images need to be placed in `public/images/` folder
- CSV data need to be placed in `public/data.csv`

Then run:

```
node ./uploader.js

# or

node run upload
```

The result json file will be saved to `./public/arweave-images.json`. This files consists of arrays of NFT objects with name / uri fields

## Result Sample

```
{
    "0": {
        "name": "ART #0000",
        "uri": "https://arweave.net/eR4wgSnWusIG-xF2BZzsiOwVehQsvfCT8VAUC4NHQ5Y"
    },
    "1": {
        "name": "ART #0001",
        "uri": "https://arweave.net/NOvV7akJDBFZogZOKxDMwIhOauiDNhVqnIfUqJmmPR8"
    },
    "2": {
        "name": "ART #0002",
        "uri": "https://arweave.net/q6RS0m0cdoieJbbXI4H1A4yJcDeFi97YF3fHVhn-h9M"
    }
}
```

[MintUI](https://github.com/InnerMindDAO/MintUI)
```
package.json
"start": "concurrently -k \"craco start\" \"npm:electron\"",
```
##MintUI Data
```
[
    "https://arweave.net/Q47yYvc2dqyS0C1cYUm6YORgic4yn-pj0rcqsNS65uQ", 

    "https://arweave.net/90DuXOCOqIwsCbxcafadFKGrzPPONWkBzPNyMUH361U", 
    
    "https://arweave.net/akaPqk9sVcwwf-4_NpwJ9rF8NsStHJ-YDDAQ7pG0Htc"

]

```

# TODO: More

-TBA
