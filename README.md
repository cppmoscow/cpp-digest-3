# cpp-digest-3

Название: C++ Дайджест №3

Дата: 4 сентября – 17 сентября 2023

## Аннотация

Привет, Хабр! Сегодня я хочу вам представить подборку интересных новостей и материалов из мира C++ за последнюю неделю.

Приятного чтения!

## ⚡️️ Новости и релизы

## 📝 Статьи

1. Andreas Fertig: [Control your numbers in C++](https://andreasfertig.blog/2023/09/control-your-numbers-in-cpp/) — Обзор нововведения C++14, для удобства чтения позволяющего использовать сепаратор в целочисленных литералах.
2. Andreas Fertig: [C++20 Dynamic Allocations at Compile Time](https://accu.org/journals/overload/31/176/overload176.pdf) — C++20 дал нам возможность выделять динамическую память в compile-time: как это работает, и какие у этой возможности есть ограничения? 
3. Arthur O'Dwyer: [Just how constexpr is C++20’s std::string?](https://quuxplusone.github.io/blog/2023/09/08/constexpr-string-firewall/) — О том, какие ограничения имеет использование `std::string` и `std::vector` в контексте времени компиляции.
4. Rainer Grimm: [C++23: Four new Associative Containers](https://www.modernescpp.com/index.php/c23-four-new-associative-containers/) — Обзор четырёх новых ассоциативных контейнеров, появившихся в C++23: `std::flat_map`, `std::flat_set`, `std::flat_multimap`, and `std::flat_multiset`. О том, когда их использование оправдано, а когда лучше использовать «классические» контейнеры.
5. Rainer Grimm: [C++23: A Multidimensional View](https://www.modernescpp.com/index.php/c23-a-multidimensional-view/) — Обзор одного из нововведений C++23, очень гибкого и кастомизируемого многомерного аналога `std::span`.
6. Marius Bancila: [Formatting Text in C++: The Old and The New Ways](https://mariusbancila.ro/blog/2023/09/12/formatting-text-in-c-the-old-and-the-new-ways/) — Обзор различных способов форматирования текста в C++, сравнение их производительности: [I/O streams](https://en.cppreference.com/w/cpp/io), семейство [printf](https://en.cppreference.com/w/cpp/io/c/fprintf) функций, [std::format](https://en.cppreference.com/w/cpp/utility/format/format), сторонняя библиотека [libfmt](https://github.com/fmtlib/fmt).
7. Sandor Dargo: [C++23: some changes related to templates](https://www.sandordargo.com/blog/2023/09/06/cpp23-templates) — Обзор нововведений C++23, благодаря которым стала возможна реализация [deducing this](https://habr.com/ru/articles/722668/): [std::forward_like](https://en.cppreference.com/w/cpp/utility/forward_like), вывод типов для унаследованных конструкторов.
8. Sandor Dargo: [Constexpr functions for smaller binary size?](https://www.sandordargo.com/blog/2023/09/13/constexpr-and-binary-sizes) — constexpr: вред или польза для размеров бинарников?
9. Raymond Chen: [How can I prevent myself from using a parameter after I’ve extracted all value from it?](https://devblogs.microsoft.com/oldnewthing/20230915-00/?p=108775)

## 📺 Видео и доклады

1. Jason Turner: [C++ Weekly - Ep 392 - Google's Bloaty McBloatface](https://www.youtube.com/watch?v=MY5DTDc3e-I) — обзор [Bloaty McBloatface: a size profiler for binaries](https://github.com/google/bloaty), поддерживающего ELF, Mach-O, PE/COFF и WebAssembly форматы бинарных файлов.
2. Jason Turner: [C++ Weekly - Ep 393 - C++23's std::unreachable](https://www.youtube.com/watch?v=ohMyb4jPIAQ) — Обзор нововведения C++23, позволяющего программисту дать компилятору подсказку о том, что некоторое место в коде недостижимо.

## 🎙️Подкасты

## Послесловие

> Дайджест составлен и опубликован при поддержке московского сообщества программистов [C++ Moscow](https://t.me/cppmoscow_info)

Заметили ошибку или опечатку? Сообщите в личку ([telegram](https://t.me/eoanermine), [habr](https://habr.com/ru/conversations/eoanermine/))

Прислать ссылку можно через форму или просто написав мне в личные сообщения ([telegram](https://t.me/eoanermine), [habr](https://habr.com/ru/conversations/eoanermine/))

← Предыдущий выпуск: [C++ Дайджест №2](https://habr.com/ru/articles/758630/)
