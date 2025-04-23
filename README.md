<div class="product">
  <img src="product-image.jpg" alt="Product Name">
  <h3>Product Name</h3>
  <p>Description of the product</p>
  <p>Price: $20</p>
  <button>Order Now</button>
</div>

let products = [
  {name: 'Shirt', price: '$15', img: 'shirt.jpg'},
  {name: 'Pants', price: '$20', img: 'pants.jpg'},
  // আরও প্রোডাক্ট
];

products.forEach(product => {
  let productDiv = document.createElement('div');
  productDiv.classList.add('product');
  
  productDiv.innerHTML = `
    <img src="${product.img}" alt="${product.name}">
    <h3>${product.name}</h3>
    <p>Price: ${product.price}</p>
    <button>Order Now</button>
  `;
  
  document.getElementById('product-list').appendChild(productDiv);
});
