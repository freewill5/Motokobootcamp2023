1. Who controls the ledger canister? = The NNS
2. What is the subnet of the canister with the id: **mwrha-maaaa-aaaab-qabqq-cai**? How much nodes are running this subnet? =  Subnet ID    16 nodes
pae4o-o6dxf-xki7q-ezclx-znyd6-fnk6w-vkv5z-5lfwh-xym2i-otrrw-fqe
3. I have a neuron with 1O ICPs locked with a dissolve delay of 4 years - my neuron has been locked for 2 years. What is my expected voting power?  = 13.25 voting power
4. What is wrong with the following code?
```
actor {
  let n : Nat = 50;
  let t : Text = "Hello";
  public func convert_to_text(m : Nat) : async Text {
    Nat.toText(m);
  };     = There is no Nat module imported. 
 
}
```
5. What is wrong with the following code?
```
actor {
  var languages : [var Text] = ["English", "German", "Chinese", "Japanese", "French"];
  public func show_languages(language : Text) : async [var Text] {
    return (languages);
  };
 
}      = The should be an immutable array  "let languages : [Text]
```
6. What is wrong with the following code?
```
actor {
  var languages : [Text] = ["English", "German", "Chinese", "Japanese", "French"];
  public func add_language(new_language: Text) : async [Text] {
    languages := Array.append<Text>(languages, [new_language]);
    return (languages);
  };
 
}    = This is missing : [var Text] to show it's mutable.