
Основные классы / функции и их применение:
- FilePGN - парсинг файлов PGN, возвращает ходы и информацию о партии (игроки, формат, ...)
- find_compatible - возвращает ход, подходящий под
- ConsoleApp - работа с командной строкой
- Position - шахматная позиция
- Stockfish - взаимодействие со Stockfish


Move is just a tuple instead of a separate class for 2 reasons:
1. Tuples are faster since it is just get-by-index, not get-by-name
2. Tuples are frozen (dataclasses can be too but slower to create)
