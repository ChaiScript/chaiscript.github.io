``` cpp
// Using ChaiScript is easy!

#include <chaiscript/chaicript.hpp>

std::string helloWorld(const std::string &t_name)
{
  return "Hello " + t_name + "!";
}

int main()
{
  chaiscript::ChaiScript chai;
  chai.add(chaiscript::fun(&helloWorld), "helloWorld");

  chai.eval("puts(helloWorld(\"Bob\"));");
}



```
