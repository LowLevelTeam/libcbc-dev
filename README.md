# COIL Byte Code Development Library

libcbc-dev is a simple extension beyond the libcoil-dev library for creating cbc for load time compilation.

Mainly used for runtime targeting of code for projects including hetregenous computing.

## Byte Code Format
The byte code format is a stack based instruction language made to be easily parseable sometimes at the sacrifice of space efficiency and complexity. Unlike COIL which focus on a simple instruction set CBC focuses on a more complex system with no type inference.

The most problematic part of JIT is the complexity in a normal trade off with higher complexity comes greater speeds with more bloat and less complexity brings slower speed simply. CBC understands this and makes it clear that CBC files will probably not be small and standard libraries with JIT functionality will be large and potentially bloated.

Light COIL variations with only some of the more standard functionality can be priotised if working with devices with minimal space like embedded devices.

## Execution
#### JIT
JIT is supported by the COIL standard library.

If you want to select a processing device at runtime then you can utilize the standard library in combination with CBC to create byte code for runtime compilation for the specific target.

#### Interpreter
CBC can also be alternatively interpreted. CBC supports being dynamic with interpretation for features such as dynamic typing for python like languages.

This is to support python to CBC for a new python interpreter which has greater support for JIT and allows for proper optional typing to be implemented.





