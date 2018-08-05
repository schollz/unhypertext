# unhypertext

unhypertext is a single webpage that can encode an entire webpage into the link. The webpage is hosted on the IPFS so its distributed.

## Instructions for setting up

```
npm install showdown lz-string
ipfs pin add $(ipfs add node_modules/showdown/dist/showdown.js | awk '{print $2}')
ipfs pin add $(ipfs add "node_modules/lz-string/libs/lz-string.js" | awk '{print $2}')
ipfs pin add $(ipfs add index.html | awk '{print $2}')
```

## License 

Unlicense
