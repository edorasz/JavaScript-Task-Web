1. Menghitung luas persegi panjang

function areaOfRectangle(length, width) {
    return length * width;
}
console.log(areaOfRectangle(5, 3)); // Output: 15
Penjelasan:

Fungsi areaOfRectangle(length, width) menerima dua parameter: panjang (length) dan lebar (width).
Menghitung luas dengan rumus length * width.
console.log(areaOfRectangle(5, 3)) memanggil fungsi dengan nilai 5 dan 3, menghasilkan output 15.


2. Menghitung diameter, keliling, dan luas lingkaran
function circleProperties(radius) {
    let diameter = 2 * radius;
    let circumference = 2 * Math.PI * radius;
    let area = Math.PI * radius * radius;
    
    console.log(`Diameter: ${diameter}, Circumference: ${circumference.toFixed(4)}, Area: ${area.toFixed(3)}`);
}
circleProperties(5); 
Penjelasan:

Fungsi circleProperties(radius) menerima parameter radius untuk menghitung:
Diameter: 2 * radius
Keliling (circumference): 2 * Math.PI * radius
Luas (area): Math.PI * radius * radius
.toFixed(n) digunakan untuk membatasi angka desimal:
circumference.toFixed(4) → 4 angka desimal
area.toFixed(3) → 3 angka desimal
Hasilnya ditampilkan dengan console.log.
Output:

Diameter: 10, Circumference: 31.4159, Area: 78.539


3. Menentukan sudut ketiga segitiga jika dua sudut diketahui
function thirdAngle(a, b) {
    return 180 - (a + b);
}
console.log(thirdAngle(80, 65)); // Output: 35
Penjelasan:

Dalam segitiga, jumlah ketiga sudut selalu 180°.
Fungsi thirdAngle(a, b) menghitung sudut ketiga dengan rumus:
Sudut ketiga = 180° - (sudut pertama + sudut kedua)
Memanggil fungsi dengan a = 80 dan b = 65 akan menghasilkan 35.


4. Menghitung selisih hari antara dua tanggal
function dateDifference(date1, date2) {
    let d1 = new Date(date1);
    let d2 = new Date(date2);
    let diffTime = Math.abs(d2 - d1);
    let diffDays = Math.ceil(diffTime / (1000 * 60 * 60 * 24));
    return diffDays;
}
console.log(dateDifference("2024-03-19", "2024-03-21")); // Output: 2
Penjelasan:

new Date(date1) dan new Date(date2) mengubah string tanggal menjadi objek Date.
d2 - d1 menghasilkan selisih waktu dalam milidetik.
Math.abs() memastikan hasilnya selalu positif.
diffTime / (1000 * 60 * 60 * 24) mengubah milidetik menjadi jumlah hari.
Math.ceil() membulatkan ke atas untuk hasil yang lebih akurat.
Output: 2


5. Mengambil inisial dari nama dan mengubahnya menjadi huruf besar
function getInitials(name) {
    return name.split(' ').map(word => word[0].toUpperCase()).join('');
}
console.log(getInitials("John Doe")); // Output: JD
Penjelasan:

name.split(' ') memisahkan nama berdasarkan spasi, menghasilkan array (["John", "Doe"]).
.map(word => word[0].toUpperCase())
Mengambil huruf pertama dari setiap kata (word[0]).
Mengubahnya menjadi huruf besar dengan .toUpperCase().
.join('') menggabungkan inisial tanpa spasi.
Output: JD
