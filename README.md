    array:read_byte
        Параметры: index (int) - Индекс элемента в массиве
        Возвращаемое значение: (int) - UInt8 значение запрашиваемого элемента
        Методы: array:read_byte(index)

    array:read_word
        Параметры: index (int) - Индекс элемента в массиве
        Возвращаемое значение: (int) - UInt16 значение запрашиваемого элемента
        Методы: array:read_word(index)

    array:read_long
        Параметры: index (int) - Индекс элемента в массиве
        Возвращаемое значение: (int) - UInt32 значение запрашиваемого элемента
        Методы: array:read_long(index)

    array:read_int64
        Параметры: index (int) - Индекс элемента в массиве
        Возвращаемое значение: (int) - UInt64 значение запрашиваемого элемента
        Методы: array:read_int64(index)

    array:size
        Возвращаемое значение: (int) - Текущее количество элементов в массиве
        Методы: array:size()
    buffer:begin
        Методы: buffer:begin()

    buffer:read_byte
        Возвращаемое значение: (int) - UInt8 значение
        Методы: buffer:read_byte()

    buffer:read_word
        Возвращаемое значение: (int) - UInt16 значение
        Методы: buffer:read_word()

    buffer:read_long
        Возвращаемое значение: (int) - UInt32 значение
        Методы: buffer:read_long()

    buffer:read_int64
        Возвращаемое значение: (int) - UInt64 значение
        Методы: buffer:read_int64()

    buffer:read_float
        Возвращаемое значение: (float) - значение с плавающей запятой
        Методы: buffer:read_float()

    buffer:read_bit
        Возвращаемое значение: (bool) - не указано
        Методы: buffer:read_bit()

    buffer:read_array
        Параметры: data (void*) - не указано, size (int) - не указано
        Возвращаемое значение: (bool) - не указано
        Методы: buffer:read_array(data, size)

    buffer:skip
        Параметры: bits (int) - не указано
        Возвращаемое значение: (bool) - не указано
        Методы: buffer:skip(bits)

    buffer:skip_to_pos
        Параметры: bits (int) - не указано
        Возвращаемое значение: (bool) - не указано
        Методы: buffer:skip_to_pos(bits)
    color (con_color) - Тип цвета (опционально)
    text (string) - Строка для вывода



    console.log(color, text)
    console.log(text)

con_color = {
    Black = 0,
    Blue = 1,
    Green = 2,
    Cyan = 3,
    Red = 4,
    Purple = 5,
    Orange = 6,
    LightGrey = 7,
    Grey = 8,
    LightBlue = 9,
    LightGreen = 10,
    LightCyan = 11,
    LightRed = 12,
    LightPurple = 13,
    Yellow = 14,
    White = 15
};
