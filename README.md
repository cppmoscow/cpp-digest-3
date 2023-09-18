# cpp-digest-3

Название: C++ Дайджест №3

Дата: 4 сентября – 17 сентября 2023

## Аннотация

Привет, Хабр! Сегодня я хочу вам представить подборку интересных новостей и материалов из мира C++ за последние две недели.

Приятного чтения!

## ⚡️️ Новости и релизы

1. [Dear ImGui 1.89.9](https://github.com/ocornut/imgui/releases/tag/v1.89.9) — Сентябрьский патч-релиз, содержащий небольшие изменения и багфиксы.
2. [Conan 1.61.0](https://github.com/conan-io/conan/releases/tag/1.61.0) — Добавление поддеркжи [SCons](https://scons.org/) и Xcode 15.
3. [Conan 2.0.11](https://github.com/conan-io/conan/releases/tag/2.0.11) — Улучшение поддеркжи [Meson](https://mesonbuild.com/) и clang-cl, исправлениие регрессий и крашей.
4. [CppCheck 2.12.0](https://sourceforge.net/p/cppcheck/news/2023/09/cppcheck-2120/) — Добавление нескольких новых и улучшение уже существующих проверок.
5. [Godot XR September 2023](https://godotengine.org/article/godot-xr-update-sep-2023/) — Добавление поддержки macOS OpenXR, нескольких новых шлемов: Tilt Five, PICO.
6. [Ogre 14.1.0](https://www.ogre3d.org/2023/09/12/ogre-14-1-released) — Добавление поддержки прямоугольных источников света и улучшение теней: теперь в их формировании может участвовать несколько светильников, а не только один.
## 📝 Статьи

1. 🇷🇺 Habr: [Собираем и запускаем калькулятор из Windows XP в среде Windows 10 c помощью GCC x64](https://habr.com/ru/articles/755752/).
2. 🇷🇺 Habr: [Создаем проект STM32 C++ FreeRTOS в VS Code для очень маленьких](https://habr.com/ru/articles/761024/) — Гайд, как подружить FreeRTOS, VS Code и C++.
3. Andreas Fertig: [Control your numbers in C++](https://andreasfertig.blog/2023/09/control-your-numbers-in-cpp/) — Обзор нововведения C++14, позволяющего использовать сепаратор в целочисленных литералах:
```c++
char buffer[2'048]{};
const auto someConstant = 2'00'00'00;
const auto anotherConstant = 0xFF'256'AF;
```
2. Andreas Fertig: [C++20 Dynamic Allocations at Compile Time](https://accu.org/journals/overload/31/176/overload176.pdf) — C++20 дал нам возможность выделять динамическую память в compile-time: как это работает, и какие у нее ограничения? 
3. Arthur O'Dwyer: [Just how constexpr is C++20’s std::string?](https://quuxplusone.github.io/blog/2023/09/08/constexpr-string-firewall/) — О том, какие ограничения имеет использование `std::string` и `std::vector` в контексте времени компиляции.
4. Rainer Grimm: [C++23: Four new Associative Containers](https://www.modernescpp.com/index.php/c23-four-new-associative-containers/) — Обзор четырёх новых ассоциативных контейнеров, появившихся в C++23: `std::flat_map`, `std::flat_set`, `std::flat_multimap`, and `std::flat_multiset`. И том, когда их использование оправдано, а когда лучше использовать «классические» контейнеры.
5. Rainer Grimm: [C++23: A Multidimensional View](https://www.modernescpp.com/index.php/c23-a-multidimensional-view/) — Обзор одного из нововведений C++23, очень гибкого и кастомизируемого многомерного аналога `std::span`.
6. Marius Bancila: [Formatting Text in C++: The Old and The New Ways](https://mariusbancila.ro/blog/2023/09/12/formatting-text-in-c-the-old-and-the-new-ways/) — Обзор различных способов форматирования текста в C++, сравнение их производительности: [I/O streams](https://en.cppreference.com/w/cpp/io), семейство [printf](https://en.cppreference.com/w/cpp/io/c/fprintf) функций, [std::format](https://en.cppreference.com/w/cpp/utility/format/format), [libfmt](https://github.com/fmtlib/fmt).
7. Sandor Dargo: [C++23: some changes related to templates](https://www.sandordargo.com/blog/2023/09/06/cpp23-templates) — Обзор нововведений C++23, благодаря которым стала возможна реализация [deducing this](https://habr.com/ru/articles/722668/): [std::forward_like](https://en.cppreference.com/w/cpp/utility/forward_like), вывод типов для унаследованных конструкторов.
8. Sandor Dargo: [Constexpr functions for smaller binary size?](https://www.sandordargo.com/blog/2023/09/13/constexpr-and-binary-sizes) — constexpr: вред или польза для размеров бинарников?
9. Julien Jorge: [Weight Gain and Perf Loss](https://julien.jorge.st/posts/en/weight-gain-and-perf-loss/) — Захватывающая детективная история об одной include-директиве, загадочным образом увеличивавшей на 5% производительность всей программы и вместе с тем уменьшавшей ее размер.
10. Daneil Lermire: [Locating ‘identifiers’ quickly (ARM NEON edition)](https://lemire.me/blog/2023/09/04/locating-identifiers-quickly-arm-neon-edition/) — Ускорение алгоритма поиска идентификаторов в строке более чем в 30 раз с помощью инструкций [ARM NEON](https://habr.com/ru/articles/548698/).


## 📺 Видео и доклады

1. Jason Turner: [C++ Weekly - Ep 392 - Google's Bloaty McBloatface](https://www.youtube.com/watch?v=MY5DTDc3e-I) — обзор [Bloaty McBloatface](https://github.com/google/bloaty), профилировщика размера для бинарных файлов, поддерживающего WebAssembly, ELF (Linux), Mach-O (MacOS) и PE/COFF (Windows).
2. Jason Turner: [C++ Weekly - Ep 393 - C++23's std::unreachable](https://www.youtube.com/watch?v=ohMyb4jPIAQ) — Обзор нововведения C++23, позволяющего программисту, недовольного недостаточным количеством неопределенного поведения в своей программе, вызвать его самостоятельно и том, зачем это иногда бывает нужно.

### C++ Now 2023

1. Daisy Hollman, Kris Jusiak: [Adapting C++20 Ranges Algorithms for Most Metaprogramming Needs in Fewer Than 1,000 Lines of Code](https://www.youtube.com/watch?v=69PuizjrgBM) — О нововведениях C++20, делающих метапрограммирование более доступным, и компромиссам между ним, кодогенерацией и дублированием.
2. Robert Seacord: [Integer Type Selection in C++: in Safe, Secure and Correct Code](https://www.youtube.com/watch?v=82jVpEmAEV4) — Гайд по выбору правильных целочисленных типов во имя красивых, удобных и безопасных интерфейсов.
3. John McCall: [Introducing a Memory-Safe Successor Language in Large C++ Code Bases](https://www.youtube.com/watch?v=lgivCGdmFrw) — О максимально безболезненном интегрировании Swift в большие плюсовые кодовые базы и том, почему именно этот язык лучше всех остальных подходит для написания критичного кода, где ошибки, связанные с неправильным управлением памятью, недопустимы.
4. David Sankel: [Assembly, System Calls, and Hardware in C++](https://www.youtube.com/watch?v=7xwjjolDnwg) — Погружение в низкоуровневые аспекты, лежащие в основе всех наших программ: системные вызовы, соглашения о вызовах, атомарные вычисления и не только.
5. Chandler Carruth: [Carbon Language Successor Strategy: From C++ Interop to Memory Safety](https://www.youtube.com/watch?v=1ZTJ9omXOQ0) — Взгляд на путь, который [Carbon](https://github.com/carbon-language/carbon-lang) предоставит для постепенного и масштабируемого обеспечения безопасности существующих плюсовых кодовых баз.
6. Tony Van Eerd: [Value Oriented Programming Part 1: You Say You Want to Write a Function](https://www.youtube.com/watch?v=b4p_tcLYDV0) — Гайд по написанию функций в value-ориентированном стиле.
7. Andrei Zissu: [Lightning Talk: A Journey Back In Time - C++ Evolution](https://www.youtube.com/watch?v=TMYW4Ohm3yI)
8. Christopher Fretz: [Lightning Talk: How Hard Can it be to SFINAE in C++03?](https://www.youtube.com/watch?v=Nf1N_vogQNM)
9. Ben Deane: [Lightning Talk: Global API Injection in C++](https://www.youtube.com/watch?v=BYpcAEfG3mo)
10. Richárd Szalay: [Lightweight Wrappers for Conscious std::transform_reduce Operation Safety](https://www.youtube.com/watch?v=cm5Zwi1EoHQ)

### Stockholm C++ 0x29

1. Paul Dreik: [Using variable templates on a tiny problem](https://www.youtube.com/watch?v=LTzpqF6wAzc) — О том, как шаблонные переменные, представленные в C++14, способны повысить удобочитаемость вашего кода.
2. Karl Åkerblom: [A quick look at Tracy Profiler](https://www.youtube.com/watch?v=W9U5y5jjQDM) — Краткий обзор инструментального профилировщика [Tracy](https://docs.flaxengine.com/manual/editor/profiling/tracy.html?tabs=code-csharp); рассмотрение нюансов работы с ним.

## 🎙️Подкасты

1. CppCast: [Episode 369, AI and Random Numbers](https://cppcast.com/ai_and_random_numbers/) — О различиях между ИИ на основе LLM и более статистических подходах, а также месте случайных чисел во всем этом и ограничениях их текущей поддержки в C++.

## Послесловие

> Дайджест составлен и опубликован при поддержке московского сообщества программистов [C++ Moscow](https://t.me/cppmoscow_info)

Заметили ошибку или опечатку? Сообщите в личку ([telegram](https://t.me/eoanermine), [habr](https://habr.com/ru/conversations/eoanermine/))

Прислать ссылку можно [через форму](https://forms.yandex.ru/cloud/64f48043e010db921819c447/) или просто написав мне в личные сообщения ([telegram](https://t.me/eoanermine), [habr](https://habr.com/ru/conversations/eoanermine/))

← Предыдущий выпуск: [C++ Дайджест №2](https://habr.com/ru/articles/758630/)
