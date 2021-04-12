# set-unicoderange

Python script to automatically set the [OpenType OS/2 table Unicode range bit flags](https://docs.microsoft.com/en-us/typography/opentype/spec/os2#ur).

## Dependencies

- Python 3.6+ interpreter
- [fontTools Python package](https://github.com/fonttools/fonttools)

## Usage

Execute the `src/set-unicoderange.py` script on the command line with one or more font path arguments.

```
$ python3 set-unicoderange.py [FONT PATH 1] (FONT PATH 2)...(FONT PATH n)
```

The script detects the code points available in the font and automatically sets the OpenType OS/2.ulUnicodeRange bit flags 1 - 4.

### Example

```
$ python3 set-unicoderange.py SomeFont-Regular.ttf
```

## License

Apache License, Version 2.0.  Please see [LICENSE](LICENSE) for details.
