# Latihan Python di Pycharm

# Cara Installasi Pycharm
1. Anda harus install Pycharm di https://www.jetbrains.com/pycharm/download/#section=windows  , Dan anda pilih yang Community
![Screenshot (76)](https://user-images.githubusercontent.com/115678171/198814989-ba36149f-cf88-492d-bb12-d00398751be4.png)
2. Anda next saja semua perintahnya 
![Screenshot (57)](https://user-images.githubusercontent.com/115794875/199217478-83d7927f-ec0d-43cb-974e-9a90e5253643.png)
Tunggu hingga selesai
![Screenshot (58)](https://user-images.githubusercontent.com/115794875/199217663-e316a809-3675-40de-8570-2c6dabc5a49e.png)


3. Jika sudah selesai maka program siap di gunakan
# Cara Menjalankan Pycharm 
# Latihan 1
1. Pertama-tama anda harus Klik New project lalu kasih nama project anda(sesuai yang anda mau), Dan anda harus pilih yang Previously Configurred interperter lalu klik yang add interperter dan pilih yang System interperter dan anda klik yang versi Python anda seperti gambar di bawah ini
![Screenshot (59)](https://user-images.githubusercontent.com/115794875/199217843-8d8cf40a-ce43-4101-9369-2a227d9b63b0.png)
![Screenshot (60)](https://user-images.githubusercontent.com/115794875/199217982-353a9399-3ee9-438f-a439-a7e81caa4904.png)


2. Selanjutnya anda membuat file Python baru di project anda tadi dan anda kasih nama file sesuai yang anda inginkan
![Screenshot (61)](https://user-images.githubusercontent.com/115794875/199218116-91b2d0bd-87f8-43c8-9d19-91e4df4e76ea.png)
Misalnya latihan1.py
![Screenshot (62)](https://user-images.githubusercontent.com/115794875/199218310-228e43c4-58f3-4132-a68b-7fe3c6c05f75.png)

3. Anda masukan code dari latihan1
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
 
![Screenshot (66)](https://user-images.githubusercontent.com/115794875/199218605-6c5ed69a-c88b-4652-9ae6-03602609a388.png)
![Screenshot (67)](https://user-images.githubusercontent.com/115794875/199218641-8bd5e99d-7209-4c70-a116-b4d5988b423b.png)

 *Lalu anda run dan ini hasilnya*
![Screenshot (68)](https://user-images.githubusercontent.com/115794875/199218733-a5c726b8-fde7-40a5-99ec-0bd117ad857f.png)
![Screenshot (69)](https://user-images.githubusercontent.com/115794875/199218806-df954ab3-19ab-4b60-bb1d-45b2648e898c.png)

# Latihan 2 
1. Anda masukan code latihan2
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
![Screenshot (70)](https://user-images.githubusercontent.com/115794875/199218977-88673386-0a96-4af6-89f8-a22c85673a1b.png)

*Berikut hasil Run*
![Screenshot (71)](https://user-images.githubusercontent.com/115794875/199219049-4ecfaa5b-946a-4f39-b3dc-2b56ca312ba3.png)

# Latihan 3
1. Anda masukan code seperti dibawah ini
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
![Screenshot (72)](https://user-images.githubusercontent.com/115794875/199219197-7ac4aaa1-8842-4534-9191-98f67db5f9f1.png)
![Screenshot (73)](https://user-images.githubusercontent.com/115794875/199219247-cc28d9b2-8355-40e2-a185-7413db9cef80.png)

*Ini hasil Run*
![Screenshot (74)](https://user-images.githubusercontent.com/115794875/199219379-06c35599-d202-46de-9f3c-b3eeeb79ee6b.png)


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
![Screenshot (76)](https://user-images.githubusercontent.com/115794875/199219471-19eb890c-624a-4c81-b7eb-cb9a1edd7e07.png)

*Dan ini hasil Run*
![Screenshot (77)](https://user-images.githubusercontent.com/115794875/199219573-302c3641-0443-4965-813a-bef3af030aa6.png)


# Flowchart Menghitung luas dan keliling lingkaran
![image](https://user-images.githubusercontent.com/115794875/199219774-4740db93-9614-487d-8aa4-52f681543d8f.png)

*Terima Kasih*

