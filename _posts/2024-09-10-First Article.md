---
title: Testing
date: 2024-09-10 12:00:00 -0500
categories: [Testing 1]
tags: [server, network, infosec]
---

# Maldev Academy

Declaring a structure 

```jsx
typedef struct _structure_name {

//structure elements

} STRUCTURE_NAME ? *PSTRUSTURE_NAME; 
```

to initialize strcuture we need to 

```jsx
STRUCTURE_NAME struct1 ={0} ; //intialize at zero 
//we can intialize a structure pointer by using NULL 

PSTRUCTURE_NAME structerpointer = NULL ; 
```

Accessing a structure  

```jsx
typedef struct _STRUCTURE_NAME {
int ID; 
int Age; 
} STRUCTURE_NAME, *PSTRUCTURE_NAME; 

STRUCTURE_NAME struct1 = {0} ; 

struct1.ID = 1000 ; // initilize the element 
struct1.Age = 34;  // initialuze  the age element 

another way is too combine them 

STRUCTURE_NAME struct1 = {.ID = 1000 , .Age=34  } ; 
```

on the other hand , accessing and initilizeing a structure its pointer is done via the arrow operator → 

```jsx
typedef stuct _STRUCTURE_NAME {
int ID; 
int Age; 
} STRUCTURE_NAME , *PSTRUCTURE_NAME; 

STRUCTURE_NAME struct1 {.ID = 1000 , .Age = 34} ; 

PSTRUTURE_NAME structurepointer = &struct1 ; 

structurepointer -> ID = 8995 ; 
printf("te strcture's ID member is now : %d \n",structureponter->ID); 

its the same as (*structurepointer).ID it is a derefrenced thing whatever . 
```

Passing by Reference : 

```jsx
void add(int *a,int *b, int *results) 
{
int A = *a
int B = *b 

*result = B + A; 
}

int main(){

int x=15 
int y =10 ; 
int sum = 0 ; 
add (&x, &y, &sum); 
return 0 ; 
}
```

- `.text` - Contains the executable code which is the written code.
- `.data` - Contains initialized data which are variables initialized in the code.
- `.rdata` - Contains read-only data. These are constant variables prefixed with `const`.
- `.idata` - Contains the import tables. These are tables of information related to the functions called using the code. This is used by the Windows PE Loader to determine which DLL files to load to the process, along with what functions are being used from each DLL.
- `.reloc` - Contains information on how to fix up memory addresses so that the program can be loaded into memory without any errors.
- `.rsrc` - Used to store resources such as icons and bitmaps

[Windows Architec ](https://www.notion.so/Windows-Architec-45fd463d7537467193a734e284606b9e?pvs=21)

[Windows memory managment](https://www.notion.so/Windows-memory-managment-f64c7ce33a2d4d8588043675281f1136?pvs=21)

[Win API](https://www.notion.so/Win-API-acaee71ab5304ef2b634378f9b8a6d10?pvs=21)

[DLLs](https://www.notion.so/DLLs-85f4b8d0877547ca976dadad6d668ccd?pvs=21)

[Advanced Detection mecanisme](https://www.notion.so/Advanced-Detection-mecanisme-01286155e97347fc839dbb88a411ebd6?pvs=21)

[Payload placement](https://www.notion.so/Payload-placement-8c7a5fe4548a44ee9ef96b89727562aa?pvs=21)

[Payload encryption and obfuscation ](https://www.notion.so/Payload-encryption-and-obfuscation-7a77b89136474f1f813f6bf609da9569?pvs=21)

[Evading microsoft satatic](https://www.notion.so/Evading-microsoft-satatic-a48c822a704c4a559f3df473a401f428?pvs=21)

[Pyload obfuscation full module  codes ](https://www.notion.so/Pyload-obfuscation-full-module-codes-18a907eeda2645e9b1ee6decd928c689?pvs=21)

[local payload execution](https://www.notion.so/local-payload-execution-0ccf892e7e93444ab11add49162208d8?pvs=21)