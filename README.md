 ```cpp
# include <iostream>
# include <stdint.h>
# include <string>
# include <memory>
# include <thread>
# include <chrono>

class Jangyubin
{
private:
	std::string		m_name = "Jangyubin";
	uint_fast64_t	m_intel = 0;

public:
	const std::string& getName(void) const
	{
		return m_name;
	}

	const uint_fast64_t& getIntel(void) const
	{
		return m_intel;
	}

	void setIntel(const uint_fast64_t& newIntel)
	{
		m_intel = newIntel;
	}

	void doStudy(void)
	{
		std::cout << " ---. " << std::endl;
		std::cout << getName() << " is studying now. " << std::endl;
		std::cout << " ---. " << std::endl;
		std::cout << std::endl;

		setIntel(getIntel() + 1);
	}
};

int main(void)
{
	std::unique_ptr<Jangyubin> me
		=
		std::make_unique<Jangyubin>();

	[&me]()
		{
			while (true)
			{
				me->doStudy();
				std::this_thread::sleep_for(std::chrono::milliseconds(25'200'000));
			}
		}();

	return 0;
}
```
---
### **Slow And Steady Wins The Race!**
### 😁😁😁
<!--
**JJangguyubin/JJangguyubin** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
