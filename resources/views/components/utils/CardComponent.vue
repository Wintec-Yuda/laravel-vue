<template>
    <div class="card">
        <img src="../../assets/logo.png" class="card-img-top img" alt="Gambar Kursus">
        <div class="card-body">
            <div class="card-title">{{ data && data.title }}</div>
            <div class="card-text">{{ data && data.creator }}</div>
            <div class="card-text">
                Duration: 2 Jam
            </div>
            <div class="card-text">
                <small class="text-muted date">25 September 2023 - 29 September 2023</small>
            </div>
        </div>
        <div class="card-footer">
            <div class="price">
                <span class="discount">Rp 100.000</span>
                <span class="original ms-2">Rp 120.000</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardComponent',
    props: {
        data: Object,
    },
}
</script>

<style scoped>
* {
    font-family: Arial, Helvetica, sans-serif;
}

.card {
    width: 250px;
    cursor: pointer;
}

.card-title {
    font-size: 18px;
    font-weight: 700;
}

.img {
    padding: 5px;
    width: auto;
    height: 150px;
    object-fit: fill;
    object-position: center;
}

.date {
    font-size: 11px;
    font-weight: 700;
}

.card-footer {
    background-color: #f7f7f7;
    text-align: center;
    padding: 10px;
}

.price {
    font-size: 24px;
    color: #333;
    font-weight: bold;
    border: rgba(0, 0, 0, 0.2) 1px solid;
    border-radius: 5px;
}

.discount {
    color: #e74c3c;
}

.original {
    text-decoration: line-through;
    color: #999;
    font-size: 14px;
    position: relative;
    top: -10px;
}
</style>
