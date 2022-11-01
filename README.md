# Latihan Python di Pycharm

# Cara Installasi Pycharm
1. Anda harus install Pycharm di https://www.jetbrains.com/pycharm/download/#section=windows  , Dan anda pilih yang Community
![Screenshot (76)](https://user-images.githubusercontent.com/115678171/198814989-ba36149f-cf88-492d-bb12-d00398751be4.png)
2. Anda next saja semua perintahnya 
3. Jika sudah selesai maka program siap di gunakan
# Cara Menjalankan Pycharm 
# Latihan 1
1. Pertama-tama anda harus Klik New project lalu kasih nama project anda(sesuai yang anda mau), Dan anda harus pilih yang Previously Configurred interperter lalu klik yang add interperter dan pilih yang System interperter dan anda klik yang versi Python anda seperti gambar di bawah ini
![Screenshot (78)](https://user-images.githubusercontent.com/115678171/198815436-8756894e-4eb0-4b58-81fe-165afda78652.png)
![Screenshot (77)](https://user-images.githubusercontent.com/115678171/198815442-dbfb3a6e-1d2f-4fdf-b205-1f7ddfb8b16c.png)

2. Selanjutnya anda membuat file Python baru di project anda tadi dan anda kasih nama file sesuai yang anda inginkan
![Screenshot (79)](https://user-images.githubusercontent.com/115678171/198815862-fbfc7ae9-dc11-4184-898a-4711596e2e7a.png)
![Screenshot (80)](https://user-images.githubusercontent.com/115678171/198815863-332a5b4f-c020-40b9-8331-4f98f5794ff9.png)

3. anda masukan code dari latihan1 anda lalu Run
```python
# penggunaan end
print('A', end='')
print('B', end='')
print('C', end='')
print()
print('X')
print('Y')
print('Z')

# penggunaan separator
w, x, y, z = 10, 15, 20, 25
print(w, x, y, z)
print(w, x, y, z, sep=',')
print(w, x, y, z, sep='')
print(w, x, y, z, sep=':')
print(w, x, y, z, sep='-----')

# string format
print(0, 10**0)
print(1, 10**1)
print(2, 10**2)
print(3, 10**3)
print(4, 10**4)
print(5, 10**5)
print(6, 10**6)
print(7, 10**7)
print(8, 10**8)
print(9, 10**9)
print(10, 10**10)

# string format
print('{0:>3} {1:>16}'.format(0, 10**0))
print('{0:>3} {1:>16}'.format(1, 10**1))
print('{0:>3} {1:>16}'.format(2, 10**2))
print('{0:>3} {1:>16}'.format(3, 10**3))
print('{0:>3} {1:>16}'.format(4, 10**4))
print('{0:>3} {1:>16}'.format(5, 10**5))
print('{0:>3} {1:>16}'.format(6, 10**6))
print('{0:>3} {1:>16}'.format(7, 10**7))
print('{0:>3} {1:>16}'.format(8, 10**8))
print('{0:>3} {1:>16}'.format(9, 10**9))
print('{0:>3} {1:>16}'.format(10, 10**10)
```
 
 ![Screenshot (63)](https://user-images.githubusercontent.com/115678171/198816032-fc8004ba-67c8-4506-954d-d7e77deac44d.png)
 ![Screenshot (64)](https://user-images.githubusercontent.com/115678171/198816037-2a855d15-28af-491f-91cd-fa16e1744518.png)
 
 *Hasil run*
 ![Screenshot (61)](https://user-images.githubusercontent.com/115678171/198816131-06a6ba95-c712-4855-8efe-264562e6b029.png)
![Screenshot (62)](https://user-images.githubusercontent.com/115678171/198816134-bc4f5b6e-d80c-4fc2-82e7-46c908987be6.png)

# Latihan 2 
1. Anda masukan code latihan 2 anda lalu Run 
```python
a=input("masukkan nilai a:")
b=input("masukkan nilai b:")
print("variable a=",a)
print("variable b=",b)
print("hasil penggabungan {1}&{0}=%s".format(a,b) %(a+b))

#koversi nilai variable
a=int(a)
b=int(b)
print("hasil penjumlahan {1}+{0}=%s".format(a,b) %(a+b))
print("hasil pembagian {1}/{0}=%s".format(a,b) %(a/b))
````
![Screenshot (68)](https://user-images.githubusercontent.com/115678171/198816300-3b5d72ee-26a4-4bf7-8fce-5710999bea71.png)
*Hasil Run*
![Screenshot (69)](https://user-images.githubusercontent.com/115678171/198816307-c1739b5e-447c-44bd-a0a2-43b3ca770e17.png)

# Latihan 3
1. Anda masukan code seperti dibawah ini dan lalu Run
```python
string = ""

x = int(input("Masukkan angka :"))
bar = x
# Looping Baris
while bar >= 0:
	# Looping Kolom Spasi Kosong
	kol = bar
	while kol > 0:
		string = string + "   "
		kol = kol - 1
	# Looping Kolom Bintang Sisi Kiri		
	kiri = 1
	while kiri < (x - (bar-1)):
		string = string + " * "
		kiri = kiri + 1		
	# Looping Kolom Bintang Sisi Kanan
	kanan = 1
	while kanan < kiri -1:
		string = string + " * "
		kanan = kanan + 1	

	string = string + "\n\n"
	bar = bar - 1

bar = 1	
# Looping Baris
while bar <= x:
	kol = bar+1
	# Looping Kolom Spasi Kosong
	while kol > 1:
		string = string + "   "
		kol = kol - 1
	# Looping Kolom Bintang Sisi Kiri	
	kiri = 0
	while kiri < (x - bar):
		string = string + " * "
		kiri = kiri + 1	
	# Looping Kolom Bintang Sisi Kanan
	kanan = kiri	
	while kanan > 1:
		string = string + " * "
		kanan = kanan - 1

	string = string + "\n\n"
	bar = bar + 1
print (string)
````
![Screenshot (71)](https://user-images.githubusercontent.com/115678171/198816679-fcdcebb6-58b9-4857-b171-2dd65952ed24.png)
![Screenshot (72)](https://user-images.githubusercontent.com/115678171/198816705-c1fbd2e3-b549-493f-8ea8-1d831895a782.png)

*Hasil Run*
![Screenshot (70)](https://user-images.githubusercontent.com/115678171/198816756-e4e3c2c0-0582-4bf4-8bdb-2f5ffc892568.png)

# Menghitung Luas Dan Keliling Lingkaran
1. Masukan code di bawah ini lalu run
```python
import math

r = float(input("Masukan Jari-jari : "))

luas = math.pi * (r * r)
keliling = 2 * math.pi * r

print("Luas Lingkaran \t\t= ", luas)
print("Keliling Lingkaran\t= ", keliling)
````
![Screenshot (82)](https://user-images.githubusercontent.com/115678171/198817214-75aca326-f313-47fe-a27c-a7fe79f08332.png)

*Hasil Run*
![Screenshot (81)](https://user-images.githubusercontent.com/115678171/198817233-c6c11b97-3aaf-48ed-b7c0-e2ff8c813896.png)

# Flowchart Menghitung luas dan keliling lingkaran
![Flowchart menghitung luas dan keliling lingkaran](https://user-images.githubusercontent.com/115678171/198817259-154fec0b-f2b1-44e5-86c0-4c7ab1ad6142.png)

*Terima Kasih*

