``locale::ffi``
===============

.. cpp:class:: ICU4XLocale

    An ICU4X Locale, capable of representing strings like ``"en-US"``. See `the Rust docs <https://unicode-org.github.io/icu4x-docs/doc/icu/locid/struct.Locale.html>`__ for more information.

    .. cpp:function:: static std::optional<ICU4XLocale> create(const std::string_view name)

        Construct an :cpp:class:`ICU4XLocale` from an locale identifier. See `the Rust docs <https://unicode-org.github.io/icu4x-docs/doc/icu/locid/struct.Locale.html#method.from_bytes>`__ for more information.

    .. cpp:function:: static ICU4XLocale create_en()

        Construct an :cpp:class:`ICU4XLocale` for the English language.

    .. cpp:function:: static ICU4XLocale create_bn()

        Construct an :cpp:class:`ICU4XLocale` for the Bangla language.

    .. cpp:function:: ICU4XLocale clone()

        Clones the :cpp:class:`ICU4XLocale`. See `the Rust docs <https://unicode-org.github.io/icu4x-docs/doc/icu/locid/struct.Locale.html>`__ for more information.

    .. cpp:function:: template<typename W> diplomat::result<std::monostate, ICU4XLocaleError> basename_to_writeable(W& write)

        Write a string representation of the ``LanguageIdentifier`` part of :cpp:class:`ICU4XLocale` to ``write``. See `the Rust docs <https://unicode-org.github.io/icu4x-docs/doc/icu/locid/struct.Locale.html#structfield.id>`__ for more information.

    .. cpp:function:: diplomat::result<std::string, ICU4XLocaleError> basename()

        Write a string representation of the ``LanguageIdentifier`` part of :cpp:class:`ICU4XLocale` to ``write``. See `the Rust docs <https://unicode-org.github.io/icu4x-docs/doc/icu/locid/struct.Locale.html#structfield.id>`__ for more information.

    .. cpp:function:: template<typename W> diplomat::result<std::monostate, ICU4XLocaleError> get_unicode_extension_to_writeable(const std::string_view bytes, W& write)

        Write a string representation of the unicode extension to ``write`` See `the Rust docs <https://unicode-org.github.io/icu4x-docs/doc/icu/locid/struct.Locale.html#structfield.extensions>`__ for more information.

    .. cpp:function:: diplomat::result<std::string, ICU4XLocaleError> get_unicode_extension(const std::string_view bytes)

        Write a string representation of the unicode extension to ``write`` See `the Rust docs <https://unicode-org.github.io/icu4x-docs/doc/icu/locid/struct.Locale.html#structfield.extensions>`__ for more information.

    .. cpp:function:: template<typename W> diplomat::result<std::monostate, ICU4XLocaleError> language_to_writeable(W& write)

        Write a string representation of :cpp:class:`ICU4XLocale` language to ``write`` See `the Rust docs <https://unicode-org.github.io/icu4x-docs/doc/icu/locid/struct.Locale.html#structfield.id>`__ for more information.

    .. cpp:function:: diplomat::result<std::string, ICU4XLocaleError> language()

        Write a string representation of :cpp:class:`ICU4XLocale` language to ``write`` See `the Rust docs <https://unicode-org.github.io/icu4x-docs/doc/icu/locid/struct.Locale.html#structfield.id>`__ for more information.

    .. cpp:function:: template<typename W> diplomat::result<std::monostate, ICU4XLocaleError> region_to_writeable(W& write)

        Write a string representation of :cpp:class:`ICU4XLocale` region to ``write`` See `the Rust docs <https://unicode-org.github.io/icu4x-docs/doc/icu/locid/struct.Locale.html#structfield.id>`__ for more information.

    .. cpp:function:: diplomat::result<std::string, ICU4XLocaleError> region()

        Write a string representation of :cpp:class:`ICU4XLocale` region to ``write`` See `the Rust docs <https://unicode-org.github.io/icu4x-docs/doc/icu/locid/struct.Locale.html#structfield.id>`__ for more information.

    .. cpp:function:: template<typename W> diplomat::result<std::monostate, ICU4XLocaleError> script_to_writeable(W& write)

        Write a string representation of :cpp:class:`ICU4XLocale` script to ``write`` See `the Rust docs <https://unicode-org.github.io/icu4x-docs/doc/icu/locid/struct.Locale.html#structfield.id>`__ for more information.

    .. cpp:function:: diplomat::result<std::string, ICU4XLocaleError> script()

        Write a string representation of :cpp:class:`ICU4XLocale` script to ``write`` See `the Rust docs <https://unicode-org.github.io/icu4x-docs/doc/icu/locid/struct.Locale.html#structfield.id>`__ for more information.

    .. cpp:function:: template<typename W> diplomat::result<std::monostate, ICU4XLocaleError> tostring_to_writeable(W& write)

        Write a string representation of :cpp:class:`ICU4XLocale` to ``write`` See `the Rust docs <https://unicode-org.github.io/icu4x-docs/doc/icu/locid/struct.Locale.html>`__ for more information.

    .. cpp:function:: diplomat::result<std::string, ICU4XLocaleError> tostring()

        Write a string representation of :cpp:class:`ICU4XLocale` to ``write`` See `the Rust docs <https://unicode-org.github.io/icu4x-docs/doc/icu/locid/struct.Locale.html>`__ for more information.

.. cpp:enum-struct:: ICU4XLocaleError

    .. cpp:enumerator:: Undefined

    .. cpp:enumerator:: Error
