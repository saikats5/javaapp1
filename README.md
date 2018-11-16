# javaapp1

javac hello.java -->(compilation) --> hello.class(java bytecode) -->java hello(interpret) --> result

JIT(just in time compilation)
identify frequently executed bytecode "hot spots"
JIT compiler coverts "hot spots" to machine code
cache machine code
cached machine code -> faster execution, also called dynamic compilation

Interpreation 
JVM instance is created --> involes sub component "class loader" locates the class and loads the bytecode to memory --> bytecode verified by bytecode verifier to ensure that loaded class file has proper internal structure and complies with the rules of java language and is critical to ensure the integrity of JVM(class files can be downloaded across the network) then it will be executed by execution engine which includes JIT compiler and interpreter, garbage collector is a component responsible for automatic memory management, security manager allows to run untrusted bytecode unless it executes dangerous operations(restrict it in sandbox environment

JRE--> only run java programs(JVM + Java API)
JDK --> develop and run java programs(Dev Tools + JVM + Java API(includes JRE))