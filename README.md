{
  "name": "learnhub",
  "version": "1.0.0",
  "description": "LearnHub - Educational Platform",
  "private": true,
  "scripts": {
    "dev": "next dev",
    "build": "next build",
    "start": "next start",
    "lint": "next lint"
  },
  "dependencies": {
    "next": "^14.0.0",
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "axios": "^1.6.0",
    "tailwindcss": "^3.3.0"
  },
  "devDependencies": {
    "eslint": "^8.50.0",
    "eslint-config-next": "^14.0.0"
  }
}
/** @type {import('next').NextConfig} */
const nextConfig = {
  reactStrictMode: true,
  swcMinify: true,
}

module.exports = nextConfig
/** @type {import('next').NextConfig} */
const nextConfig = {
  reactStrictMode: true,
  swcMinify: true,
}

module.exports = nextConfig
import '../styles/globals.css'

export default function App({ Component, pageProps }) {
  return <Component {...pageProps} />
}export default function Home() {
  return (
    <div className="min-h-screen bg-gradient-to-br from-blue-50 to-indigo-100">
      {/* Navigation */}
      <nav className="bg-white shadow-sm">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="flex justify-between items-center h-16">
            <div className="flex items-center">
              <h1 className="text-2xl font-bold text-indigo-600">🎓 LearnHub</h1>
            </div>
            <div className="flex gap-4">
              <button className="px-4 py-2 text-indigo-600 hover:text-indigo-800">
                تسجيل الدخول
              </button>
              <button className="px-4 py-2 bg-indigo-600 text-white rounded-lg hover:bg-indigo-700">
                التسجيل الآن
              </button>
            </div>
          </div>
        </div>
      </nav>

      {/* Hero Section */}
      <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-20 text-center">
        <h2 className="text-5xl font-bold text-gray-900 mb-6">
          منصة التعليم التفاعلية 🚀
        </h2>
        <p className="text-xl text-gray-600 mb-8 max-w-2xl mx-auto">
          تعلم المهارات الجديدة من خبراء العالم، احصل على شهادات معترف بها، وانضم لمجتمع من المتعلمين
        </p>
        <button className="bg-indigo-600 text-white px-8 py-3 rounded-lg text-lg font-semibold hover:bg-indigo-700 transition">
          ابدأ التعلم الآن
        </button>
      </div>

      {/* Features */}
      <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-16">
        <h3 className="text-3xl font-bold text-center mb-12">المميزات الرئيسية</h3>
        <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
          {[
            { title: '🎥 دروس فيديوية', desc: 'محتوى عالي الجودة من خبراء' },
            { title: '🏆 شهادات معترف بها', desc: 'احصل على شهادات رسمية' },
            { title: '💬 منتدى تفاعلي', desc: 'تواصل مع المعلمين والطلاب' },
            { title: '📊 متابعة التقدم', desc: 'لوحة تحكم شخصية متطورة' },
            { title: '🌐 دعم لغات', desc: 'العربية والإنجليزية وغيرها' },
            { title: '💳 دفع آمن', desc: 'معالجة دفع آمنة وموثوقة' }
          ].map((feature, i) => (
            <div key={i} className="bg-white p-6 rounded-lg shadow hover:shadow-lg transition">
              <h4 className="text-lg font-semibold mb-2">{feature.title}</h4>
              <p className="text-gray-600">{feature.desc}</p>
            </div>
          ))}
        </div>
      </div>

      {/* Footer */}
      <footer className="bg-gray-900 text-white py-12 mt-20">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
          <p>© 2026 LearnHub. جميع الحقوق محفوظة</p>
        </div>
      </footer>
    </div>
  )
}/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    './pages/**/*.{js,ts,jsx,tsx}',
    './components/**/*.{js,ts,jsx,tsx}',
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}# Learn
Learn
