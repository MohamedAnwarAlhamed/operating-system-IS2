# operating-system-IS2
1) Create folders and files.
mkdir D
cd D
mkdir D{1 . . 4}
touch F1
cd D4
touch F41
cd ..
cd D3
mkdir D{31..33}
cd D33
touch F331
cd ..
cd D32
mkdir D321
cd ..
cd D31
mkdir D311 D312
cd ../..
cd D2
mkdir D21
cd D21
touch F211
cd ../..
cd D1
mkdir D11 D12
touch F11
cd D11
mkdir D{111..113}
cd D111
touch F1111
cd ..
cd D112
touch F1121
cd ..
cd D113
touch F1131
cd ../..
cd D12
mkdir D121 D122
cd D121
touch F1212 F1211
2)Copy the file F1131 To D321.
cd D/D1/D11/D113
cp F1131 ../../../D3/D32/321
3)Copy the F1131 To file1.
cd D/D1/D11/D113
cp F1131 ../../../F1
4)Copy folder contents D121 To D311 folder.
cd D/D1/D12
cp -r D121 ../../D3/D31/D311
5)Copy the file F1212 and F1211 To D2 folder.
cd D/D1/D12/D121
cp F1212 F1211 ../../../D2
6)Rename the file F1111 To FFFF.
cd D/D1/D11/D111
mv F1111 FFFF
7)Move the files F1212 and F1211 To D4.
cd D/D1/D12/D121
mv F1212 F1211 ../../../D4
8)Remove the file F11.
cd D/D1
rm F11
9)Remove folder contents D3
cd D
rm -rf D3
10) do soft and hard linking for file F331 in a desktop path.
 Soft linking:
cd Desktop
ln -s ~/D/D3/D33/F331 F332
 Hard linking:
cd Desktop
ln ~/D/D3/D33/F331 F333
