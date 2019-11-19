# peace
Piece Table in Go

## Explanation
The piece table is an immutable data structure that allows for the quick and efficient editing of text buffers.
Because of it's immutable nature it is also efficient when implementing unlimited undo and redo.
One thing I sought after with a text buffer was the lowest memory footprint possible and piece table/chains seem to be the best for the use case.
For more explanation on how this all works, please see the resources section below.

#### Current Implementation

Currently the piece table is implemented using a doubly-linked list.
The performance has not been measure but is most likely not great at the moment.

#### Enhancements/Roadmap/TODO

- [ ] Implement more public methods
  - [ ] List here...
- [ ] Implement using a AVL/Red-Black Tree for lookups
- [ ] Implement unlimited redo and undo
- [ ] Measure peformance bottlenecks for what needs to be optimized
- [ ] Compare against other text buffers
- [ ] Write Tests for most everything
- [ ] Test Unicode ability 
- [ ] more...


#### Resources

 - [VSCode Text Buffer](https://code.visualstudio.com/blogs/2018/03/23/text-buffer-reimplementation)
 - [Wikipedia Page Description](https://en.wikipedia.org/wiki/Piece_table)
 - [Neatpad Article (Piece Chains)](http://www.catch22.net/tuts/neatpad/piece-chains#)
 - [Atom Text Buffer](https://blog.atom.io/2017/10/12/atoms-new-buffer-implementation.html)
 - [Good Blog Article](https://www.averylaird.com/programming/the%20text%20editor/2017/09/30/the-piece-table/)
 - [Sequence Data Structure Paper](https://www.cs.unm.edu/~crowley/papers/sds.pdf)
 - [Oberon OS System](https://inf.ethz.ch/personal/wirth/ProjectOberon/PO.System.pdf)
 - [Abiword Text Buffer](http://www.abisource.com/wiki/AbiWordDevelopment#PieceTableBackground)
 - [Abiword Text Buffer Improved](http://e98cuenc.free.fr/wordprocessor/piecetable.html)