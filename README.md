#Bson.ml

**Bson.ml** is an ocaml module that includes a Bson document data structure, together with its encoding (to bytes) and decoding (from bytes). 

The logic of **usage** is like this

1. Create an empty Bson document
2. Create the elements you want
3. Add elements to the document with names
4. Or remove elements from the document via the names
5. Get elements from the document via the names
6. After obtaining an element, get the raw value from the element

The functions inside this module seem to be many, however, most of them are just for creating elements. These functions are to *hide the implementation details of the type elements*. Also, in this way, the Bson document can be used more safely.

	In order to taste Bson.ml, please have a look at test/test_bson.ml. 
    You can use the following command in the root of the project to run it:

	ocamlbuild -I src test/test_ocaml_bson.native
	./test_ocaml_bson.native 


Please also refer to the [Official Bson specification](http://bsonspec.org/#/specification) for more information.

*Version 0.88.0* 

*Yes, I would like to call this utility as Bson.ml instead of ocamlbson, or something like that.* 

*In addition, experienced ocaml developers are welcomed to improve the code base*

