- 👋 Hi, I’m @sfjs929
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fotoğraf Yarışması</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Fotoğraf Yarışması</h1>
    <h2>Kategori: En Güzel Çiçek</h2>
    <div id="photo-container" class="photo-container"></div>
    <script src="script.js"></script>
</body>
</html>body {
    font-family: Arial, sans-serif;
    text-align: center;
    background-color: #f0f0f0;
}

h1, h2 {
    color: #333;
}

.photo-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
    padding: 20px;
}

.photo-card {
    background-color: white;
    border-radius: 10px;
    padding: 10px;
    width: 200px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.photo-card img {
    width: 100%;
    height: auto;
    border-radius: 5px;
}

.photo-card p {
    margin: 5px 0;
}

button {
    background-color: #4CAF50;
    color: white;
    border: none;
    padding: 5px 10px;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background-color: #45a049;
}
<!---// Örnek fotoğraf verileri (gerçek uygulamada bu bir veritabanından gelir)
let photos = [
    { id: 1, url: "https://via.placeholder.com/200?text=Cicek1", likes: 15, title: "Gül" },
    { id: 2, url: "https://via.placeholder.com/200?text=Cicek2", likes: 25, title: "Papatya" },
    { id: 3, url: "https://via.placeholder.com/200?text=Cicek3", likes: 10, title: "Lale" }
];

// Fotoğrafları beğeni sayısına göre sıralayıp ekrana yerleştirme
function displayPhotos() {
    photos.sort((a, b) => b.likes - a.likes); // Beğeni sayısına göre azalan sıralama
    const container = document.getElementById("photo-container");
    container.innerHTML = ""; // Önceki içeriği temizle

    photos.forEach(photo => {
        const photoCard = document.createElement("div");
        photoCard.className = "photo-card";
        photoCard.innerHTML = `
            <img src="${photo.url}" alt="${photo.title}">
            <p>${photo.title}</p>
            <p>Beğeni: <span id="likes-${photo.id}">${photo.likes}</span></p>
            <button onclick="likePhoto(${photo.id})">Beğen</button>
        `;
        container.appendChild(photoCard);
    });
}

// Beğenme fonksiyonu
function likePhoto(id) {
    const photo = photos.find(p => p.id === id);
    photo.likes += 1;
    displayPhotos(); // Yeniden sırala ve göster
}

// Sayfa yüklendiğinde fotoğrafları göster
window.onload = displayPhotos;
sfjs929/sfjs929 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
