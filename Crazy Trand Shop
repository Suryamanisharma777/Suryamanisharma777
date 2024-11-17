const CrazyTrandShop = () => {
  const [searchQuery, setSearchQuery] = useState('');
  const [cartItems, setCartItems] = useState([]);

  const categories = [
    'Electronics', 'Fashion', 'Home & Furniture', 'Beauty & Personal Care',
    'Appliances', 'Toys & Games', 'Sports', 'Books'
  ];

  const featuredProducts = [
    {
      id: 1,
      name: 'Smartphone Pro Max',
      price: 599.99,
      originalPrice: 799.99,
      discount: '25%',
      rating: 4.5,
      image: '/api/placeholder/200/200'
    },
    {
      id: 2,
      name: 'Premium Wireless Earbuds',
      price: 129.99,
      originalPrice: 199.99,
      discount: '35%',
      rating: 4.3,
      image: '/api/placeholder/200/200'
    },
    {
      id: 3,
      name: 'Smart Watch Series X',
      price: 299.99,
      originalPrice: 399.99,
      discount: '25%',
      rating: 4.7,
      image: '/api/placeholder/200/200'
    },
  ];

  const Logo = () => (
    <svg viewBox="0 0 24 24" className="h-8 w-8 text-white">
      <path
        fill="currentColor"
        d="M21 9h-2V7h2v2zm-4-4V3h6v6h-2V7h-2v2h-2V5h-2zM3 19v2h2v-2H3zm4 2h2v-2H7v2zm4 0h2v-2h-2v2zm4 0h2v-2h-2v2zm4 0h2v-2h-2v2zM3 7v2h2V7H3zm0 4v2h2v-2H3zm0 4v2h2v-2H3zm4-8v2h2V7H7zm0 4v2h2v-2H7zm0 4v2h2v-2H7z"
      />
    </svg>
  );

  const ProductCard = ({ product }) => (
    <div className="bg-white p-4 rounded-lg shadow hover:shadow-lg transition-shadow">
      <img
        src={product.image}
        alt={product.name}
        className="w-full h-48 object-contain mb-4"
      />
      <h3 className="font-medium text-lg mb-2">{product.name}</h3>
      <div className="flex items-center gap-2 mb-2">
        <span className="text-xl font-bold">${product.price}</span>
        <span className="text-gray-500 line-through text-sm">${product.originalPrice}</span>
        <span className="text-green-600 text-sm">{product.discount} off</span>
      </div>
      <div className="flex items-center gap-1">
        <span className="bg-green-600 text-white px-2 py-1 rounded text-sm">
          {product.rating} ★
        </span>
        <span className="text-gray-500 text-sm">(1,234 reviews)</span>
      </div>
    </div>
  );

  return (
    <div className="min-h-screen bg-gray-100">
      <header className="bg-gradient-to-r from-gray-900 to-gray-800 text-white">
        <div className="max-w-7xl mx-auto px-4">
          <div className="py-4 flex items-center gap-8">
            <div className="flex-shrink-0 flex items-center gap-3">
              <Logo />
              <div>
                <h1 className="text-2xl font-bold" style={{ color: '#D4AF37' }}>CRAZY TRAND SHOP</h1>
                <p className="text-xs text-gray-400">Everyone should need to show craziness</p>
              </div>
            </div>

            <div className="flex-grow">
              <div className="flex">
                <input
                  type="text"
                  placeholder="Search for products, brands and more"
                  className="w-full px-4 py-2 text-black rounded-l focus:outline-none"
                  value={searchQuery}
                  onChange={(e) => setSearchQuery(e.target.value)}
                />
                <button className="bg-orange-500 px-8 rounded-r hover:bg-orange-600">
                  <Search className="h-5 w-5" />
                </button>
              </div>
            </div>

            <nav className="flex items-center gap-6">
              <button className="flex items-center gap-2 hover:text-gray-300">
                <User className="h-5 w-5" />
                <span>Login</span>
              </button>
              <button className="flex items-center gap-2 hover:text-gray-300">
                <ShoppingCart className="h-5 w-5" />
                <span>Cart</span>
              </button>
              <button className="hover:text-gray-300">
                <Heart className="h-5 w-5" />
              </button>
              <button className="hover:text-gray-300">
                <Bell className="h-5 w-5" />
              </button>
            </nav>
          </div>

          <div className="py-2">
            <ul className="flex justify-between">
              {categories.map((category) => (
                <li key={category}>
                  <button className="flex items-center gap-1 hover:text-gray-300 px-2 py-1">
                    {category}
                    <ChevronDown className="h-4 w-4" />
                  </button>
                </li>
              ))}
            </ul>
          </div>
        </div>
      </header>

      <main className="max-w-7xl mx-auto px-4 py-8">
        <div className="mb-8">
          <img
            src="/api/placeholder/1200/300"
            alt="Main Banner"
            className="w-full h-64 object-cover rounded-lg shadow"
          />
        </div>

        <section className="mb-12">
          <h2 className="text-2xl font-bold mb-6">Featured Categories</h2>
          <div className="grid grid-cols-2 md:grid-cols-4 gap-4">
            {categories.slice(0, 4).map((category) => (
              <div
                key={category}
                className="bg-white rounded-lg shadow p-6 text-center hover:shadow-lg transition-shadow cursor-pointer"
              >
                <img
                  src="/api/placeholder/100/100"
                  alt={category}
                  className="w-24 h-24 mx-auto mb-4"
                />
                <h3 className="font-medium">{category}</h3>
              </div>
            ))}
          </div>
        </section>

        <section className="mb-12">
          <div className="flex items-center justify-between mb-6">
            <h2 className="text-2xl font-bold">Deals of the Day</h2>
            <button className="bg-gradient-to-r from-gray-900 to-gray-800 text-white px-6 py-2 rounded hover:opacity-90">
              View All
            </button>
          </div>
          <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
            {featuredProducts.map((product) => (
              <ProductCard key={product.id} product={product} />
            ))}
          </div>
        </section>

        <section>
          <h2 className="text-2xl font-bold mb-6">Top Picks For You</h2>
          <div className="grid grid-cols-1 md:grid-cols-4 gap-4">
            {[...featuredProducts, ...featuredProducts.slice(0, 1)].map((product, index) => (
              <ProductCard key={`top-${product.id}-${index}`} product={product} />
            ))}
          </div>
        </section>
      </main>

      <footer className="bg-gradient-to-r from-gray-900 to-gray-800 text-white py-12">
        <div className="max-w-7xl mx-auto px-4">
          <div className="grid grid-cols-1 md:grid-cols-4 gap-8">
            <div>
              <h3 className="text-lg font-bold mb-4">About</h3>
              <ul className="space-y-2">
                <li className="hover:text-gray-300 cursor-pointer">Contact Us</li>
                <li className="hover:text-gray-300 cursor-pointer">About Us</li>
                <li className="hover:text-gray-300 cursor-pointer">Careers</li>
                <li className="hover:text-gray-300 cursor-pointer">Press</li>
              </ul>
            </div>
            <div>
              <h3 className="text-lg font-bold mb-4">Help</h3>
              <ul className="space-y-2">
                <li className="hover:text-gray-300 cursor-pointer">Payments</li>
                <li className="hover:text-gray-300 cursor-pointer">Shipping</li>
                <li className="hover:text-gray-300 cursor-pointer">Returns</li>
                <li className="hover:text-gray-300 cursor-pointer">FAQ</li>
              </ul>
            </div>
            <div>
              <h3 className="text-lg font-bold mb-4">Policy</h3>
              <ul className="space-y-2">
                <li className="hover:text-gray-300 cursor-pointer">Return Policy</li>
                <li className="hover:text-gray-300 cursor-pointer">Terms of Use</li>
                <li className="hover:text-gray-300 cursor-pointer">Security</li>
                <li className="hover:text-gray-300 cursor-pointer">Privacy</li>
              </ul>
            </div>
            <div>
              <h3 className="text-lg font-bold mb-4">Social</h3>
              <ul className="space-y-2">
                <li className="hover:text-gray-300 cursor-pointer">Facebook</li>
                <li className="hover:text-gray-300 cursor-pointer">Twitter</li>
                <li className="hover:text-gray-300 cursor-pointer">Instagram</li>
                <li className="hover:text-gray-300 cursor-pointer">YouTube</li>
              </ul>
            </div>
          </div>
          <div className="border-t border-gray-700 mt-8 pt-8 text-center">
            <p>&copy; 2024 CRAZY TRAND SHOP. All rights reserved.</p>
          </div>
        </div>
      </footer>
    </div>
  );
};

export default CrazyTrandShop;
