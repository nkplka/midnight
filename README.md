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
        draw.get_window_width()
        Parameters: None
        Return Value: Returns the width of the game window in pixels (integer).

    draw.get_window_height()
        Parameters: None
        Return Value: Returns the height of the game window in pixels (integer).

    draw.get_screen_width()
        Parameters: None
        Return Value: Returns the width of the screen in pixels (integer).

    draw.get_screen_height()
        Parameters: None
        Return Value: Returns the height of the screen in pixels (integer).

    draw.create_texture_from_file(file_name)
        Parameters:
            file_name (string): The path to the image file.
        Return Value: Returns a handle to the created texture (integer).

    draw.create_texture_from_memory(ptr, size)
        Parameters:
            ptr (integer): The memory address of the image data.
            size (integer): The size of the image data in bytes.
        Return Value: Returns a handle to the created texture (integer).

    draw.release_texture(handle)
        Parameters:
            handle (integer): The handle of the texture to release.
        Return Value: None

    draw.set_hsv(ctx_color, h, s, v, a)
        Parameters:
            ctx_color (integer): The context color to modify.
            h (float): The hue value (0.0 to 1.0).
            s (float): The saturation value (0.0 to 1.0).
            v (float): The value/brightness value (0.0 to 1.0).
            a (float): The alpha/transparency value (0.0 to 1.0).
        Return Value: None

    draw.set_hsv(ctx_color, h, s, v)
        Parameters:
            ctx_color (integer): The context color to modify.
            h (float): The hue value (0.0 to 1.0).
            s (float): The saturation value (0.0 to 1.0).
            v (float): The value/brightness value (0.0 to 1.0).
        Return Value: None

    draw.set_color(ctx_color, rgba)
        Parameters:
            ctx_color (integer): The context color to modify.
            rgba (integer): The color value in RGBA format (32-bit unsigned integer).
        Return Value: None

    draw.set_color(ctx_color, r, g, b, a)
        Parameters:
            ctx_color (integer): The context color to modify.
            r (integer): The red component of the color (0 to 255).
            g (integer): The green component of the color (0 to 255).
            b (integer): The blue component of the color (0 to 255).
            a (integer): The alpha component of the color (0 to 255).
        Return Value: None

    draw.set_color(ctx_color, r, g, b)
        Parameters:
            ctx_color (integer): The context color to modify.
            r (integer): The red component of the color (0 to 255).
            g (integer): The green component of the color (0 to 255).
            b (integer): The blue component of the color (0 to 255).
        Return Value: None

    draw.get_color(ctx_color)
        Parameters:
            ctx_color (integer): The context color to retrieve.
        Return Value: Returns the color value in RGBA format (32-bit unsigned integer).

    draw.set_thickness(thickness)
        Parameters:
            thickness (float): The thickness value for drawing operations.
        Return Value: None
    entity.spawn_ped

Parameters:

    hash (string/number)
    position (Vector3)
    on_spawned (function)

Methods:

    entity.spawn_ped(hash, position, on_spawned)
    entity.spawn_ped(hash, position)
    entity.spawn_ped(hash, on_spawned)
    entity.spawn_ped(hash)

Callbacks:

    function on_spawned(entity)

entity.spawn_veh

Parameters:

    hash (string/number)
    position (Vector3)
    on_spawned (function)

Methods:

    entity.spawn_veh(hash, position, on_spawned)
    entity.spawn_veh(hash, position)
    entity.spawn_veh(hash, on_spawned)
    entity.spawn_veh(hash)

Callbacks:

    function on_spawned(entity)

entity.spawn_cloud_veh

Parameters:

    name (string)
    position (Vector3)
    on_spawned (function)

Methods:

    entity.spawn_cloud_veh(name, position, on_spawned)
    entity.spawn_cloud_veh(name, position)
    entity.spawn_cloud_veh(name, on_spawned)
    entity.spawn_cloud_veh(name)

Callbacks:

    function on_spawned(entity)

entity.spawn_obj

Parameters:

    hash (string/number)
    position (Vector3)
    on_spawned (function)

Methods:

    entity.spawn_obj(hash, position, on_spawned)
    entity.spawn_obj(hash, position)
    entity.spawn_obj(hash, on_spawned)
    entity.spawn_obj(hash)

Callbacks:

    function on_spawned(entity)

entity.delete

Parameters:

    entity (int)
    on_failed (function)
    on_deleted (function)

Methods:

    entity.delete(entity, on_deleted, on_failed)
    entity.delete(entity, on_deleted)
    entity.delete(entity)

Callbacks:

    function on_failed(entity)
    function on_deleted(entity)

entity.is_controlled

Parameters:

    entity (int)

Return Value:

    success (bool)

Methods:

    entity.is_controlled(entity)

entity.request_control

Parameters:

    entity (int)
    on_obtain (function)
    tag (optional)

Methods:

    entity.request_control(entity, on_obtain, tag)
    entity.request_control(entity, on_obtain)
    entity.request_control(entity)

Callbacks:

    function on_obtain(entity, tag)
    function on_obtain(entity)

entity.get_owner

Parameters:

    entity (int)

Return Value:

    owner (number)

Methods:

    entity.get_owner(entity)
