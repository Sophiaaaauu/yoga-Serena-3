import { Button } from ‘./components/Button’; import { BenefitCard } from ‘./components/BenefitCard’; import { ExperienceCard } from ‘./components/ExperienceCard’; import { TestimonialCard } from ‘./components/TestimonialCard’; import { ProductCard } from ‘./components/ProductCard’; import { ImageWithFallback } from ‘./components/figma/ImageWithFallback’; import { Sparkles, Heart, Flower2, Instagram, Mail, Phone } from ‘lucide-react’; import yogaVideo from ‘../imports/WhatsApp_Video_2026-05-21_at_1.33.56_PM.mp4’; import logoImage from ‘../imports/image-4.png’; import kitSerenaImage from ‘../imports/image-5.png’;

export default function App() {

return ( <div className="min-h-screen bg-[#FAF7F2]"> {/* Navbar */} <nav className="fixed top-0 left-0 right-0 z-50 transition-all duration-300 backdrop-blur-md bg-white/30"> <div className="max-w-7xl mx-auto px-6 py-4 flex justify-between items-center"> <div className="flex items-center gap-3"> <ImageWithFallback src={logoImage} alt=”Yoga Serena Logo” className=”h-14 w-auto object-contain” /> <h1 className=”font-serif text-2xl tracking-wide text-[#5A5A5A] uppercase” style=> Yoga Serena </h1> </div> <div className="hidden md:flex gap-8"> Nuestras Experiencias Beneficios Testimonios </div> </div> </nav>

  {/* Hero Section */}
  <section className="relative h-screen flex items-center justify-center overflow-hidden">
    <div className="absolute inset-0">
      <img
        src="https://images.unsplash.com/photo-1772543149976-6d6de951616a?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHwxfHxtaW5pbWFsaXN0JTIwbWVkaXRhdGlvbiUyMHNlcmVuZSUyMHdvbWFufGVufDF8fHx8MTc3ODYxNzYxOHww&ixlib=rb-4.1.0&q=80&w=1080"
        alt="Mujer meditando"
        className="w-full h-full object-cover"
      />
      <div className="absolute inset-0 bg-[#E8DDD0]/40"></div>
    </div>
    <div className="relative z-10 text-center px-6 max-w-4xl">
      <ImageWithFallback
        src={logoImage}
        alt="Yoga Serena"
        className="h-32 md:h-40 w-auto object-contain mx-auto mb-8"
      />
      <h1 className="font-serif text-5xl md:text-7xl text-[#5A5A5A] leading-tight">
        Reconecta con tu feminidad,<br />
        libérate del estrés y<br />
        despierta tu potencial.
      </h1>
    </div>
  </section>

  {/* Misión y Visión Section */}
  <section className="py-24 px-6 bg-white">
    <div className="max-w-6xl mx-auto">
      <div className="grid md:grid-cols-2 gap-16">
        <div className="bg-gradient-to-br from-[#F5D7D9]/30 to-[#E8DDD0]/30 rounded-3xl p-12 hover:shadow-xl transition-all duration-300">
          <div className="flex items-center gap-3 mb-6">
            <span className="text-4xl">🌿</span>
            <h2 className="font-serif text-4xl text-[#5A5A5A]">Misión</h2>
          </div>
          <p className="text-[#5A5A5A]/80 text-lg leading-relaxed">
            En Yoga Serena creamos experiencias de bienestar que conectan cuerpo, mente y emociones a través del yoga, la meditación y rituales sensoriales, brindando un espacio de calma, autocuidado y equilibrio para mujeres que desean reconectar consigo mismas.
          </p>
        </div>
        <div className="bg-gradient-to-br from-[#B8C5B3]/30 to-[#F5D7D9]/30 rounded-3xl p-12 hover:shadow-xl transition-all duration-300">
          <div className="flex items-center gap-3 mb-6">
            <span className="text-4xl">✨</span>
            <h2 className="font-serif text-4xl text-[#5A5A5A]">Visión</h2>
          </div>
          <p className="text-[#5A5A5A]/80 text-lg leading-relaxed">
            Ser una marca de bienestar reconocida en Bogotá por inspirar una vida más consciente, femenina y equilibrada, creando una comunidad que encuentre en Yoga Serena un refugio de tranquilidad, conexión y amor propio.
          </p>
        </div>
      </div>
    </div>
  </section>

  {/* Beneficios Section */}
  <section id="beneficios" className="py-24 px-6 bg-gradient-to-b from-[#FAF7F2] to-[#F5D7D9]/10">
    <div className="max-w-7xl mx-auto">
      <h2 className="font-serif text-5xl text-center text-[#5A5A5A] mb-20">
        Beneficios que transforman
      </h2>
      <div className="grid md:grid-cols-3 gap-12">
        <BenefitCard
          icon={<Sparkles size={32} />}
          title="Reduce el estrés"
          description="Libera las tensiones acumuladas y encuentra paz interior a través de prácticas conscientes diseñadas para tu bienestar."
        />
        <BenefitCard
          icon={<Heart size={32} />}
          title="Reconecta contigo"
          description="Redescubre tu esencia femenina y fortalece la conexión con tu cuerpo, mente y espíritu en un espacio seguro."
        />
        <BenefitCard
          icon={<Flower2 size={32} />}
          title="Bienestar emocional"
          description="Cultiva el equilibrio emocional y la armonía interior para vivir con plenitud y serenidad cada día."
        />
      </div>
    </div>
  </section>

  {/* Experiencias Section */}
  <section id="experiencias" className="py-24 px-6">
    <div className="max-w-7xl mx-auto">
      <h2 className="font-serif text-5xl text-center text-[#5A5A5A] mb-8">
        Nuestras experiencias
      </h2>
      <p className="text-center text-[#5A5A5A]/70 mb-20 max-w-2xl mx-auto text-lg">
        Cada experiencia está diseñada para nutrir tu cuerpo, calmar tu mente y despertar tu espíritu.
      </p>
      <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
        <ExperienceCard
          image="https://images.unsplash.com/photo-1768430826748-e5c1c9faf643?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHwyfHxtaW5pbWFsaXN0JTIwbWVkaXRhdGlvbiUyMHNlcmVuZSUyMHdvbWFufGVufDF8fHx8MTc3ODYxNzYxOHww&ixlib=rb-4.1.0&q=80&w=1080"
          title="🧘‍♀️ Yoga consciente"
          description="Sesiones diseñadas para conectar cuerpo, mente y respiración en un espacio de calma y equilibrio. Ayuda a reducir el estrés, mejorar la flexibilidad y fortalecer el bienestar emocional."
        />
        <ExperienceCard
          image="https://images.unsplash.com/photo-1743112943399-fc221eefd181?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHwzfHxtaW5pbWFsaXN0JTIwbWVkaXRhdGlvbiUyMHNlcmVuZSUyMHdvbWFufGVufDF8fHx8MTc3ODYxNzYxOHww&ixlib=rb-4.1.0&q=80&w=1080"
          title="🌙 Meditación guiada"
          description="Experiencias de meditación enfocadas en liberar tensión mental y encontrar paz interior. Favorece la concentración, disminuye la ansiedad y aporta claridad emocional."
        />
        <ExperienceCard
          image="https://images.unsplash.com/photo-1576287251622-0eb2f24ae759?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHwxfHx3ZWxsbmVzcyUyMHNwYSUyMGNhbmRsZXMlMjBhcm9tYXRoZXJhcHl8ZW58MXx8fHwxNzc4NjE3NjE3fDA&ixlib=rb-4.1.0&q=80&w=1080"
          title="✨ Ritual sensorial"
          description="Una experiencia de bienestar con aromas, música y mindfulness para reconectar contigo misma. Relaja profundamente, estimula los sentidos y ayuda a equilibrar las emociones."
        />
        <ExperienceCard
          image={kitSerenaImage}
          title="🎁 Kit Serena"
          description="Un kit premium creado para llevar la esencia de Yoga Serena a tu rutina diaria. Promueve el autocuidado, crea momentos de calma y transforma tu espacio en un refugio de bienestar."
          linkTo="#productos"
        />
      </div>
    </div>
  </section>

  {/* Sección Sensorial */}
  <section className="py-16 px-6 bg-white">
    <div className="max-w-5xl mx-auto">
      <div className="grid md:grid-cols-2 gap-12 items-center">
        <div className="space-y-6">
          <h2 className="font-serif text-4xl text-[#5A5A5A] leading-tight">
            Una experiencia<br />
            para todos tus sentidos
          </h2>
          <p className="text-[#5A5A5A]/70 leading-relaxed">
            Cada detalle está cuidadosamente diseñado para envolverte en una atmósfera de calma y lujo.
            Velas aromáticas, aceites esenciales naturales, texturas suaves y una iluminación cálida
            crean el ambiente perfecto para tu transformación interior.
          </p>
          <a href="#productos">
            <Button variant="secondary">
              Explora nuestros productos
            </Button>
          </a>
        </div>
        <div className="grid grid-cols-2 gap-3">
          <img
            src="https://images.unsplash.com/photo-1706795033917-dee116e7cba2?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHw1fHx3ZWxsbmVzcyUyMHNwYSUyMGNhbmRsZXMlMjBhcm9tYXRoZXJhcHl8ZW58MXx8fHwxNzc4NjE3NjE3fDA&ixlib=rb-4.1.0&q=80&w=600"
            alt="Velas aromáticas"
            className="rounded-2xl shadow-md hover:shadow-lg transition-all duration-300 hover:scale-105 h-32 w-full object-cover"
          />
          <img
            src="https://images.unsplash.com/photo-1607914660217-754fdd90041d?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHw1fHxvdXRkb29yJTIweW9nYSUyMG5hdHVyZSUyMHdvbWFuJTIwcGVhY2VmdWx8ZW58MXx8fHwxNzc4Nzg4NjQzfDA&ixlib=rb-4.1.0&q=80&w=600"
            alt="Yoga al aire libre"
            className="rounded-2xl shadow-md hover:shadow-lg transition-all duration-300 hover:scale-105 mt-4 h-32 w-full object-cover"
          />
          <img
            src="https://images.unsplash.com/photo-1674600628997-7acb4200735b?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHw1fHx5b2dhJTIwbWF0JTIwZXNzZW50aWFsJTIwb2lscyUyMGxpZmVzdHlsZXxlbnwxfHx8fDE3Nzg2MTc2MTh8MA&ixlib=rb-4.1.0&q=80&w=600"
            alt="Mat de yoga"
            className="rounded-2xl shadow-md hover:shadow-lg transition-all duration-300 hover:scale-105 mt-6 h-32 w-full object-cover"
          />
          <img
            src="https://images.unsplash.com/photo-1687875495230-96dfea96d9da?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHw0fHx3b21lbiUyMG1lZGl0YXRpb24lMjBncm91cCUyMGNpcmNsZXxlbnwxfHx8fDE3Nzg3ODg3MzN8MA&ixlib=rb-4.1.0&q=80&w=600"
            alt="Clase grupal de yoga"
            className="rounded-2xl shadow-md hover:shadow-lg transition-all duration-300 hover:scale-105 mt-2 h-32 w-full object-cover"
          />
        </div>
      </div>
    </div>
  </section>

  {/* Productos Section */}
  <section id="productos" className="py-24 px-6 bg-gradient-to-b from-white to-[#FAF7F2]">
    <div className="max-w-7xl mx-auto">
      <h2 className="font-serif text-5xl text-center text-[#5A5A5A] mb-8">
        Kit Serena
      </h2>
      <p className="text-center text-[#5A5A5A]/70 mb-20 max-w-2xl mx-auto text-lg">
        Todo lo que necesitas para tu bienestar en un solo kit premium. Elementos cuidadosamente seleccionados para elevar tu práctica.
      </p>
      <div className="grid md:grid-cols-2 lg:grid-cols-3 gap-8 mb-12">
        <ProductCard
          image="https://images.unsplash.com/photo-1743798578464-f0b09d79aaa4?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHw5fHxleGVyY2lzZSUyMG1hdCUyMGZpdG5lc3MlMjBwaW5rJTIwcHVycGxlfGVufDF8fHx8MTc3ODc5MDk4MXww&ixlib=rb-4.1.0&q=80&w=1080"
          title="Mat de Yoga"
          description="Mat premium con diseño antideslizante, perfecto para tu práctica diaria con estilo y comodidad."
        />
        <ProductCard
          image="https://images.unsplash.com/photo-1603006905003-be475563bc59?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHwyfHxhcm9tYXRpYyUyMGNhbmRsZXMlMjBhZXN0aGV0aWMlMjBmZW1pbmluZXxlbnwxfHx8fDE3Nzg3OTA3MDV8MA&ixlib=rb-4.1.0&q=80&w=1080"
          title="Vela Aromática"
          description="Vela artesanal con aromas naturales que transforman tu espacio en un refugio de calma."
        />
        <ProductCard
          image="https://images.unsplash.com/photo-1767605529955-4c6e192b5c12?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHwzfHxpbmNlbnNlJTIwc3RpY2tzJTIwd2VsbG5lc3MlMjBhcm9tYXRoZXJhcHl8ZW58MXx8fHwxNzc4NzkwNzA2fDA&ixlib=rb-4.1.0&q=80&w=1080"
          title="Inciensos"
          description="Inciensos naturales de alta calidad para purificar tu espacio y profundizar tu meditación."
        />
        <ProductCard
          image="https://images.unsplash.com/photo-1676852148076-7a92002419f3?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHwyfHxlc3NlbnRpYWwlMjBvaWxzJTIwYm90dGxlJTIwbmF0dXJhbCUyMG9yZ2FuaWN8ZW58MXx8fHwxNzc4NzkwNzA2fDA&ixlib=rb-4.1.0&q=80&w=1080"
          title="Aceite Esencial"
          description="Aceite 100% puro y natural para aromaterapia, masajes y cuidado personal consciente."
        />
        <ProductCard
          image="https://images.unsplash.com/photo-1732963947955-858ad7d5e540?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHwyfHx0b3RlJTIwYmFnJTIwY2FudmFzJTIwYmVpZ2UlMjBtaW5pbWFsaXN0JTIwYWVzdGhldGljfGVufDF8fHx8MTc3OTIyMDk0Mnww&ixlib=rb-4.1.0&q=80&w=1080"
          title="Tote Bag Yoga Serena"
          description="Bolsa de lona premium con el logo de Yoga Serena, perfecta para llevar tus esenciales de bienestar."
        />
        <ProductCard
          image="https://images.unsplash.com/photo-1605714312496-01e90cb509cc?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHw0fHxtaW5pbWFsaXN0JTIwd2hpdGUlMjB0aGVybW9zJTIwYWVzdGhldGljJTIwcHJvZHVjdHxlbnwxfHx8fDE3NzkyMjEwOTJ8MA&ixlib=rb-4.1.0&q=80&w=1080"
          title="Termo Blanco"
          description="Termo térmico elegante para mantener tu hidratación en cada práctica y durante todo el día."
        />
      </div>
      <div className="text-center">
        <a href="https://wa.me/573157308588?text=Hola%20%F0%9F%8C%BF%0AQuisiera%20recibir%20m%C3%A1s%20informaci%C3%B3n%20sobre%20las%20experiencias%20y%20servicios%20de%20Yoga%20Serena%20%E2%9C%A8%F0%9F%A4%8D" target="_blank" rel="noopener noreferrer">
          <Button variant="primary" className="text-lg px-16 py-5">
            Consultar disponibilidad
          </Button>
        </a>
      </div>
    </div>
  </section>

  {/* Testimonios */}
  <section id="testimonios" className="py-24 px-6 bg-gradient-to-b from-[#FAF7F2] to-[#B8C5B3]/10">
    <div className="max-w-7xl mx-auto">
      <h2 className="font-serif text-5xl text-center text-[#5A5A5A] mb-20">
        Historias de transformación
      </h2>
      <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
        <TestimonialCard
          image="https://images.unsplash.com/photo-1773757807865-8635ef353be2?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHwxfHx3b21hbiUyMHlvZ2ElMjBzdW5yaXNlJTIwcGVhY2VmdWwlMjBuYXR1cmV8ZW58MXx8fHwxNzc4NjE3NjE2fDA&ixlib=rb-4.1.0&q=80&w=400"
          name="Carolina Mendoza"
          comment="Yoga Serena me ayudó a encontrar la paz que tanto necesitaba. Cada sesión es un regalo para mi alma."
        />
        <TestimonialCard
          image="https://images.unsplash.com/photo-1627840237551-a1116348e0e1?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHw1fHxtaW5pbWFsaXN0JTIwbWVkaXRhdGlvbiUyMHNlcmVuZSUyMHdvbWFufGVufDF8fHx8MTc3ODYxNzYxOHww&ixlib=rb-4.1.0&q=80&w=400"
          name="Sofía Rivera"
          comment="Después de años desconectada de mí misma, aquí encontré mi centro. Un espacio de amor y cuidado genuino."
        />
        <TestimonialCard
          image="https://images.unsplash.com/photo-1761030448313-b73fef243958?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHw0fHx3b21hbiUyMHlvZ2ElMjBzdW5yaXNlJTIwcGVhY2VmdWwlMjBuYXR1cmV8ZW58MXx8fHwxNzc4NjE3NjE2fDA&ixlib=rb-4.1.0&q=80&w=400"
          name="Valentina Torres"
          comment="La experiencia sensorial es increíble. Salgo de cada sesión renovada, como si hubiera renacido."
        />
        <TestimonialCard
          image="https://images.unsplash.com/photo-1644718847160-52a922094f69?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w3Nzg4Nzd8MHwxfHNlYXJjaHwyfHx5b3VuZyUyMHdvbWFuJTIwcGVhY2VmdWwlMjBjYWxtJTIwcG9ydHJhaXQlMjBuYXR1cmFsfGVufDF8fHx8MTc3ODc4OTYwNXww&ixlib=rb-4.1.0&q=80&w=400"
          name="Laura Martínez"
          comment="Entre el trabajo y la universidad había perdido el tiempo para mí y mi feminidad. Yoga Serena me ayudó a sentirme más tranquila, segura y en equilibrio otra vez."
        />
      </div>
    </div>
  </section>

  {/* Video Section */}
  <section className="py-24 px-6 bg-white">
    <div className="max-w-5xl mx-auto">
      <h2 className="font-serif text-5xl text-center text-[#5A5A5A] mb-16">
        Tips antes de tu clase de yoga
      </h2>
      <div className="relative rounded-3xl overflow-hidden shadow-2xl bg-[#F5D7D9]/10 p-4">
        <video
          className="w-full rounded-2xl"
          controls
          preload="metadata"
          src={yogaVideo}
        >
          Tu navegador no soporta el elemento de video.
        </video>
      </div>
    </div>
  </section>

  {/* Instagram Section */}
  <section className="py-24 px-6 bg-gradient-to-b from-white to-[#FAF7F2]">
    <div className="max-w-7xl mx-auto text-center">
      <a href="https://instagram.com/yogaserenaa" target="_blank" rel="noopener noreferrer" className="inline-flex items-center justify-center gap-3 mb-12 hover:opacity-80 transition-opacity">
        <Instagram className="text-[#B8C5B3]" size={32} />
        <h2 className="font-serif text-5xl text-[#5A5A5A]">
          @yogaserenaa
        </h2>
      </a>
      <p className="text-[#5A5A5A]/70 mb-16 text-lg">
        Únete a nuestra comunidad de bienestar
      </p>
      <div className="grid grid-cols-2 md:grid-cols-4 gap-4">
        {[
          'https://images.unsplash.com/photo-1566501206188-5dd0cf160a0e?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=400',
          'https://images.unsplash.com/photo-1713201673819-122ab540f947?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=400',
          'https://images.unsplash.com/photo-1635751254361-30f09bc7f820?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=400',
          'https://images.unsplash.com/photo-1667890785988-8da12fd0989b?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=400',
        ].map((img, i) => (
          <a key={i} href="https://instagram.com/yogaserenaa" target="_blank" rel="noopener noreferrer" className="aspect-square rounded-3xl overflow-hidden hover:scale-105 transition-transform duration-300 cursor-pointer block">
            <img src={img} alt="Instagram" className="w-full h-full object-cover" />
          </a>
        ))}
      </div>
    </div>
  </section>

  {/* CTA Final */}
  <section className="py-32 px-6 bg-[#B8C5B3]/20">
    <div className="max-w-4xl mx-auto text-center space-y-8">
      <h2 className="font-serif text-6xl text-[#5A5A5A] leading-tight">
        Haz una pausa para ti.
      </h2>
      <p className="text-[#5A5A5A]/70 text-xl leading-relaxed max-w-2xl mx-auto">
        Tu bienestar merece ser prioridad. Regálate un momento de conexión profunda y
        descubre la versión más serena de ti misma.
      </p>
      <a href="https://wa.me/573157308588?text=Hola%20%F0%9F%8C%BF%0AQuisiera%20recibir%20m%C3%A1s%20informaci%C3%B3n%20sobre%20las%20experiencias%20y%20servicios%20de%20Yoga%20Serena%20%E2%9C%A8%F0%9F%A4%8D" target="_blank" rel="noopener noreferrer">
        <Button variant="primary" className="text-xl px-12 py-5">
          Reserva ahora
        </Button>
      </a>
    </div>
  </section>

  {/* Footer */}
  <footer className="bg-[#E8DDD0] py-16 px-6">
    <div className="max-w-7xl mx-auto">
      <div className="grid md:grid-cols-3 gap-12 mb-12">
        <div>
          <ImageWithFallback
            src={logoImage}
            alt="Yoga Serena Logo"
            className="h-20 w-auto object-contain mb-4"
          />
          <p className="text-[#5A5A5A]/70 italic mb-4">
            "Cada respiración es una oportunidad para reconectarte contigo misma."
          </p>
          <p className="text-[#5A5A5A]/70">
            📍 Ubicados en Bogotá, Colombia
          </p>
        </div>
        <div>
          <h4 className="font-medium text-[#5A5A5A] mb-4">Contacto</h4>
          <div className="space-y-3 text-[#5A5A5A]/70">
            <a href="https://instagram.com/yogaserenaa" target="_blank" rel="noopener noreferrer" className="flex items-center gap-2 hover:text-[#5A5A5A] transition-colors">
              <Instagram size={18} />
              <span>@yogaserenaa</span>
            </a>
            <a href="mailto:yogaserenaa@gmail.com" className="flex items-center gap-2 hover:text-[#5A5A5A] transition-colors">
              <Mail size={18} />
              <span>yogaserenaa@gmail.com</span>
            </a>
            <a href="https://wa.me/573157308588" target="_blank" rel="noopener noreferrer" className="flex items-center gap-2 hover:text-[#5A5A5A] transition-colors">
              <Phone size={18} />
              <span>+57 3157308588</span>
            </a>
          </div>
        </div>
        <div>
          <h4 className="font-medium text-[#5A5A5A] mb-4">Escríbenos</h4>
          <div className="flex gap-4">
            <a href="https://instagram.com/yogaserenaa" target="_blank" rel="noopener noreferrer" className="w-10 h-10 rounded-full bg-white/50 flex items-center justify-center hover:bg-white transition-colors">
              <Instagram size={20} className="text-[#5A5A5A]" />
            </a>
            <a href="https://wa.me/573157308588" target="_blank" rel="noopener noreferrer" className="w-10 h-10 rounded-full bg-white/50 flex items-center justify-center hover:bg-white transition-colors">
              <Phone size={20} className="text-[#5A5A5A]" />
            </a>
          </div>
        </div>
      </div>
      <div className="border-t border-[#5A5A5A]/10 pt-8 text-center text-[#5A5A5A]/70">
        <p>© 2026 Yoga Serena. Todos los derechos reservados.</p>
      </div>
    </div>
  </footer>
</div>   ); }
