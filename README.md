# Lua Minimum Spanning Tree
Generates a minimum spanning tree in Lua given a graph of edges

# Installation
Add mst.lua to your project folder and call it with require

# Usage
mst.lua provides 1 function, 
````
mst.tree 
````
which accepts a list of the vertices of the graph with the list entries in the form of {x1,y1} and a list of the lines between the vertices of the graph with the list entries in the form of {x1,y1,x2,y2}, returning a list of the edges of the tree in the form {x1,y1,x2,y2}

# Example
````
mst = require 'mst'
points = {{1,2},{2,3},{3,4}}
edges = {{1,2,2,3},{2,3,3,4},{3,4,1,2}}
tree = mst.tree(points,edges)
for i = 1, #tree do
  print(tree[i][1],tree[i][2],tree[i][3],tree[i][4])
end
--prints each edge of the tree as x1,y1,x2,y2
````
##License
This work is under [MIT-LICENSE](http://www.opensource.org/licenses/mit-license.php).<br/>
Copyright (c) 2017 Anders Sundheim

    Permission is hereby granted, free of charge, to any person obtaining a
    copy of this software and associated documentation files (the
    "Software"), to deal in the Software without restriction, including
    without limitation the rights to use, copy, modify, merge, publish,
    distribute, sublicense, and/or sell copies of the Software, and to
    permit persons to whom the Software is furnished to do so, subject to
    the following conditions:

    The above copyright notice and this permission notice shall be included
    in all copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
    OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
    MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
    IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
    CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
    TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
    SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
