# Namespaces
A namespace is a mapping from names to objects.

## Lifetime of a namespace
1. The namespace containing the built-in names is created when the Python interpreter starts up, and is never deleted.
2. The global namespace for a module is created when the module definition is read in; normally, module namespaces also last until the interpreter quits.
3. The local namespace for a function is created when the function is called, and deleted when the function returns or raises an exception that is not handled within the function.

# Scope
A scope is a textual region of a Python program where a namespace is directly accessible. “Directly accessible” here means that an unqualified reference to a name attempts to find the name in the namespace.

Although scopes are determined statically, they are used dynamically.At any time during execution, At any time during execution, there are 3 or 4 nested scopes whose namespaces are directly accessible:
1. The innermost scope, which is searched first, contains the local names
2. The scopes of any enclosing functions, which are searched starting with the nearest enclosing scope, contains non-local, but also non-global names
3. The next-to-last scope contains the current module’s global names
4. The outermost scope (searched last) is the namespace containing built-in names

# Attribute
Strictly speaking, references to names in modules are attribute references: in the expression modname.funcname, modname is a module object and funcname is an attribute of it
