<template>
  <div class="home">

    <!-- Header -->
    <header class="header">
      <div class="menu">☰</div>
      <h1 class="logo">ReVeste</h1>
      <div class="icons">
        🔔 🛒
      </div>
    </header>

    <!-- Search -->
    <div class="search-container">
      <input type="text" placeholder="Search items..." />
      <span class="search-icon">🔍</span>
      <span class="filter-icon">⚲</span>
    </div>

    <!-- Banner -->
    <div class="banner">
      <div class="banner-text">
        <h2>20% Off</h2>
        <p>on your first 2 orders!</p>
        <small>PROMO CODE: XA45762ZQ</small>
        <button>Shop now »</button>
      </div>
    </div>

    <!-- Categories -->
    <section class="categories">
      <div
        class="category"
        v-for="cat in categories"
        :key="cat"
      >
        <div class="circle"></div>
        <span>{{ cat }}</span>
      </div>
    </section>

    <!-- For you -->
    <section class="products">
      <h2>Para você</h2>

      <div class="product-list">
        <div
          class="product"
          v-for="product in products"
          :key="product.name"
        >
          <img :src="product.image" />
          <p>{{ product.name }}</p>
        </div>
      </div>
    </section>

    <!-- Bottom Navigation -->
    <nav class="bottom-nav">
      <span>🏠</span>
      <span>⬜</span>
      <span>👤</span>
    </nav>

  </div>
</template>

<script>
export default {
  name: "HomePage",
  data() {
    return {
      categories: [
        "Casual",
        "Streetwear",
        "Formal",
        "Vintage",
        "Kids",
        "Praia",
        "Esporte",
        "Verão",
        "Inverno"
      ],
      products: [
        {
          name: "1pc Plain Black Sports",
          image: "https://via.placeholder.com/120"
        },
        {
          name: "1pc Plain White Polo",
          image: "https://via.placeholder.com/120"
        },
        {
          name: "1pc Plain Black Hoodie",
          image: "https://via.placeholder.com/120"
        }
      ]
    };
  }
};
</script>

<style scoped>

.home {
  font-family: Arial, sans-serif;
  padding-bottom: 70px;
}

/* HEADER */

.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 16px;
}

.logo {
  font-family: serif;
  font-size: 28px;
}

.icons {
  display: flex;
  gap: 10px;
}

/* SEARCH */

.search-container {
  display: flex;
  align-items: center;
  margin: 0 16px 16px;
  position: relative;
}

.search-container input {
  width: 100%;
  padding: 10px 40px;
  border-radius: 20px;
  border: 1px solid #ccc;
}

.search-icon {
  position: absolute;
  left: 12px;
}

.filter-icon {
  position: absolute;
  right: 12px;
}

/* BANNER */

.banner {
  margin: 0 16px;
  border-radius: 16px;
  padding: 20px;
  color: white;
  background: linear-gradient(
    90deg,
    #222,
    #555
  );
}

.banner-text h2 {
  font-size: 32px;
  margin: 0;
}

.banner-text button {
  margin-top: 10px;
  padding: 6px 12px;
  border: none;
  border-radius: 6px;
}

/* CATEGORIES */

.categories {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  gap: 12px;
  padding: 20px 16px;
  text-align: center;
}

.category {
  font-size: 12px;
}

.circle {
  width: 40px;
  height: 40px;
  border: 1px solid #ccc;
  border-radius: 50%;
  margin: auto;
  margin-bottom: 6px;
}

/* PRODUCTS */

.products {
  padding: 0 16px;
}

.products h2 {
  margin-bottom: 12px;
}

.product-list {
  display: flex;
  gap: 12px;
}

.product {
  width: 110px;
}

.product img {
  width: 100%;
  border-radius: 8px;
}

/* BOTTOM NAV */

.bottom-nav {
  position: fixed;
  bottom: 0;
  width: 100%;
  height: 60px;
  border-top: 1px solid #ddd;
  background: white;

  display: flex;
  justify-content: space-around;
  align-items: center;

  font-size: 22px;
}

</style>