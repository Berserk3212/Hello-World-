// char_subst.cpp
#include <iostream>
#include <cstdlib>
using namespace std;

// Читаем из потока ввода символы и пишем их в поток вывода,
// подменяя некоторые на другие (e -> i, o -> u, a -> o).
int main()
{
  for (char ch; cin.get(ch);)
  {
    char output = ch;
    if (ch == 'e')
      output = 'i';
    else if (ch == 'o')
      output = 'u';
    else if (ch == 'a')
      output = 'o';
    cout.put(output);
  }
  return EXIT_SUCCESS;
}
