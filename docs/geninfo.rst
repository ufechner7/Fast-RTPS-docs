Introduction
============

eProsima FASTRTPSGEN is a Java application that generates source code using the data types defined in an IDL file. This generated source code can be used in your applications in order to publish and subscribe to a topic of your defined type.

To declare your structured data, you have to use IDL (Interface Definition Language) format. IDL is a specification language, made by OMG (Object Management Group), which describes an interface in a language-independent way, enabling communication between software components that do not share the same language.

eProsima FASTRTPSGEN is a tool that reads IDL files and parses a subset of the OMG IDL specification to generate serialization source code. This subset includes the data type descriptions included in section 3. The rest of the file content is ignored.

eProsima FASTRTPSGEN generated source code uses a relevant component: a C++11 library that provides a serialization mechanism. In this case, as indicated by the RTPS specification document, the serialization mechanism used in CDR. The standard CDR (Common Data Representation)1 is a transfer syntax low-level representation for transfer between agents, mapping from data types defined in OMG IDL to byte streams. 

One of the main features of eProsima FASTRTPSGEN is to avoid the users the trouble of knowing anything about serialization or deserialization procedures. It also provides a first implementation of a publisher and a subscriber using eProsima RTPS library.
This document presents a brief guide of how to use eProsima FASTRTPSGEN. The structure of the document is presented below:

