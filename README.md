# JAVA HASHCODE BREAKER

# Motivation

The most popular and powerful tools such as [Hashcat](https://github.com/hashcat)
or [John The Ripper](https://www.openwall.com/john/) used to be as default
hash cracking tools. But to some unknown reasons neither hashcat no john couldn't crack simple Java Object hashcode
function. And even a lot of instruments couldn't identify such type of hash. This is very strange because sometimes Java
developers converts users passwords with simple hashcode function and pushes in to database which make dictionary
attack reasonable. Also, if you don't want to pay to crack you hash on resources
as [Hashes.com](https://hashes.com/en/credits) you may use this tool for testing.

### Some additional information
[Hashcat: issue Java hashCode() Token Length Exception with Hex integer](https://github.com/hashcat/hashcat/issues/3559)

![simple_java_hash.png](assets%2Fsimple_java_hash.png)
![hash_unknown_hash.png](assets%2Fhash_unknown_hash.png)
![hashid_unknown_hash.png](assets%2Fhashid_unknown_hash.png)
![hashcat_unknown_hash.png](assets%2Fhashcat_unknown_hash.png)
![john_unknown_hash.png](assets%2Fjohn_unknown_hash.png)

# Usage
1. Clone the repository
2. Change path to builds 
    ```
    cd java_hashcode_breaker/builds
    ```
3. Run .jar file with options below
    ```
    java -jar <current build vesion>.jar -h <provide hash here> -w <path to wordlist>
   ```
4. You can add -v option for verbose output 
    ```
    java -jar <current build vesion>.jar -h <provide hash here> -w <path to wordlist> -v
    ```
5. Happy cracking.

### Example of work
Without verbosity

![example.png](assets%2Fexample.png)

With -v option

![example_verbose.png](assets%2Fexample_verbose.png)


