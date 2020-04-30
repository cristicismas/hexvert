#!/usr/bin/python

from sys import argv

def to_string(hex):
    return hex.decode('utf-8')

def to_edian(edian_type, hex_string):
    return int(hex_string[2:], 16).to_bytes(4, edian_type)

def main():
    if len(argv) != 3:
        print("Usage: hexvert <hex> <string|little|big>")
        exit(1)
    else:
        hex_string = argv[1]
        convert_to = argv[2]

        if convert_to == "string":
            little_edian = to_edian("little", hex_string)
            string = to_string(little_edian)

            print(string)
        elif convert_to == "little":
            print(to_edian("little", hex_string))
        elif convert_to == "big":
            print(to_edian("big", hex_string))
        else:
            print("The second argument must be either \"string\", \"little\", or \"big\"")
            exit(1)
        
        exit(0)

if __name__ == "__main__":
    main()
