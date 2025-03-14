'''cpp
# include <iostream>

// using namespace std;

int main(void) {

	auto showMyMottos =
		[]() {
		std::cout << " --- " << std::endl;
		std::cout << " <My mottos> " << std::endl;
		std::cout
			<< " 1. 盡人事待天命. "
			<< std::endl
			<< " 2. Slow and steady wins the race. "
			<< std::endl;
		std::cout << " --- " << std::endl;
		std::cout << std::endl;
		};

	showMyMottos();

	return 0;
}
'''
