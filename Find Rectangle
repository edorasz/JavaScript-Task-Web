// 1. Menghitung luas persegi panjang
function areaOfRectangle(length, width) {
    return length * width;
}
console.log(areaOfRectangle(5, 3)); // Output: 15

// 2. Menghitung diameter, keliling, dan luas lingkaran
function circleProperties(radius) {
    let diameter = 2 * radius;
    let circumference = 2 * Math.PI * radius;
    let area = Math.PI * radius * radius;
    
    console.log(`Diameter: ${diameter}, Circumference: ${circumference.toFixed(4)}, Area: ${area.toFixed(3)}`);
}
circleProperties(5); 
// Output: Diameter: 10, Circumference: 31.4159, Area: 78.539

// 3. Menentukan sudut ketiga segitiga jika dua sudut diketahui
function thirdAngle(a, b) {
    return 180 - (a + b);
}
console.log(thirdAngle(80, 65)); // Output: 35

// 4. Menghitung selisih hari antara dua tanggal
function dateDifference(date1, date2) {
    let d1 = new Date(date1);
    let d2 = new Date(date2);
    let diffTime = Math.abs(d2 - d1);
    let diffDays = Math.ceil(diffTime / (1000 * 60 * 60 * 24));
    return diffDays;
}
console.log(dateDifference("2024-03-19", "2024-03-21")); // Output: 2

// 5. Mengambil inisial dari nama dan mengubahnya menjadi huruf besar
function getInitials(name) {
    return name.split(' ').map(word => word[0].toUpperCase()).join('');
}
console.log(getInitials("John Doe")); // Output: JD
