all:
	clang main2.cpp
check1:
	clang-tidy main.cpp

fmt:
	clang-format -i *.cpp
s:
	clang main2.cpp \
		-fstack-protector \
		-fstack-protector-strong \
		-fstack-protector-all \
		-fsanitize=safe-stack \
		-D_DORTIFY_SOURCE=1 -O0 \
		-fcf-protection=full \
		-fsanitize=cfi -flto -fvisibility=hidden \
		-fsplit-stack \
		-fno-stack-arrays \
		-Wframe-larger-than=1000 \
		-Walloca \
		-Walloca-larger-than \
		-Wvla -Wvla-larger-than \
		-fstack-usage \
		-Wstack-usage
