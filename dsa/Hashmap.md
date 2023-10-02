> HashTables are the thread-safe counterpart

Resources:
- SimonDev: [Hash Tables, Associative Arrays, and Dictionaries](https://youtube.com/watch?v=S5NY1fqisSY)

## Rehashing

## Collisions
### Linear Probing / Open Addressing
This technique, when **inserting**, if a collision is found, the next open address is instead used. e.g. hashed key maps to position `4` but `4` is filled with a different hash, we check `5` to see if its free. We keep going x+1 until we find a free location. When **accessing** we do the same thing but instead we're looking for our match.
> When searching, the worst case scenario is that we need to search the entire hashMap. But this is unlikely if the hash function is chosen well. Rehashing can also help with this

## Javascript Objects
In javascript, objects are hashMaps/tabls and they seem to use linear probing to resolve collisions. I can't find the initial size of objects, but the `Map`class seems to use 16 by default.