# JOURNAL-I

## Send your passphrase-encrypted files to ipfs or shout your message public

This is a linux terminal script made for launching files to ipfs, either encrypted (_whisper_) or public (_shout_) and listen to ipfs documents already encrypted (_listen_). This a basic guide for installing, setup and use. You can use `journal-i --help` or `journal-i -h` for more help.


## Sendind simple documents to the network (shout)

```
$ journal-i -s mydocument.doc
$ journal-i --shout mydocument.doc
```

This will launch a normal document to the network, the only thing anyone needs to read it is the _ipfs hash_ but it doesn't have a password. The file will divide into _ipfs blocks_ and sitribute into the chosen network (normal gateway or infura).

## Sending encrypted documents to the network (whisper)

```
$ journal-i -w mydocument.doc -p mypassword
$ journal-i --whisper mydocument.doc -p mypassword
```

Thiw will launch an encrypted document to the network. Even having the hash, if someone doesn't know the password, the content wont be visible.

## Retrieving encrypted documents from the network (listen)

```
$ journal-i -l hash -p password -o output
$ journal-i --listen -p password -o output
```

This will get the content of the hash and ask for the password, in order to read or open it.


_Note: The script isn't finished yet._
