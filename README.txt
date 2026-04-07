## TODO / wishlist

- smth to take apart and reassemble a CD image from the command line cross-platform
  - image-analyzer works for extracting data (ISO9660) and audio tracks (WAV) from CloneCD data (.ccd + .img), but is GUI, and doesn't seem capable of reassembling that data

### `fmt-builder.py` and `fmt-extractor.py`

Scripts for working with the packed files found on the PC-98 CD release of Ballade for Maria, and the FM Towns release of Dead of the Brain.

In Ballade of Maria:

- maria.000
- maria.001
- ...
- maria.045

With maria.000 starting like this:

```
00000000: 6d61 7269 612e 6469 7200 0000 7400 0000  maria.dir...t...
00000010: 6d61 7269 612e 6364 7400 0000 b20b 0000  maria.cdt.......
00000020: 6d61 7269 612e 6d66 7400 0000 c50b 0000  maria.mft.......
00000030: 6d61 7269 612e 7365 0000 0000 a70c 0000  maria.se........
00000040: 6964 6573 3935 2e67 7063 0000 421e 0000  ides95.gpc..B...
00000050: 0000 0000 0000 0000 0000 0000 fc2d 0000  .............-..
00000060: 841b b31e 5596 a81e ea95 ad1e 0060 9c1e  ....U........`..
00000070: 0060 9c1e 6d61 7269 6100 0000 7374 6172  .`..maria...star
00000080: 7400 0000 0100 7365 6c65 6374 0000 0100  t.....select....
```

Taken from https://github.com/slowbeef/dotb-romhack, with adjustments for Linux compatibility.
