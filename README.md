// Next.js 14 (App Router) - Landing Page Inicial da Mérito Autocuidado
// Estrutura base do projeto para deploy imediato na Vercel
// Observação: Este arquivo representa apenas a landing page (app/page.js)
import Image from "next/image";
import meritoLogo from "../public/merito-logo.png"; // substitua pelo arquivo real
export default function Home() {
  return (
    <main className="min-h-screen bg-white text-gray-800">
      {/* Hero Section */}
      <section className="flex flex-col items-center justify-center text-center py-24 px-6 bg-gradient-to-b from-white to-gray-100">
        <Image src={meritoLogo} alt="Mérito Autocuidado" width={140} height={140} />
        <h1 className="text-4xl font-bold mt-8 mb-4 text-gray-900">
          Transformando Saúde em Valor
        </h1>
        <p className="text-lg max-w-2xl text-gray-600 mb-8">
          A primeira plataforma que converte seus exames de saúde em um score que te presenteia com CoinSaúde — a moeda digital que recompensa o autocuidado.
        </p>
        <div className="flex gap-4">
          <a href="#usuario" className="px-6 py-3 rounded-xl bg-blue-600 text-white font-medium">
            Criar Minha Conta
          </a>
          <a href="#Usuario" className="px-6 py-3 rounded-xl bg-gray-200 text-gray-900 font-medium">
            Sou Usuario
          </a>
        </div>
      </section>
      {/* Como Funciona */}
      <section id="como-funciona" className="py-20 px-6 bg-white text-center">
        <h2 className="text-3xl font-semibold mb-10">Como Funciona</h2>
        <div className="grid grid-cols-1 md:grid-cols-3 gap-10 max-w-5xl mx-auto">
          <div>
            <h3 className="text-xl font-semibold mb-2">1. Faça seus exames de saúde</h3>
            <p className="text-gray-600">Realize seu check-up em qualquer laboratório credenciado ou envie os exames de sangue para a plataforma.</p>
          </div>
          <div>
            <h3 className="text-xl font-semibold mb-2">2. Receba seu Score Mérito</h3>
            <p className="text-gray-600">A Mérito analisa seus indicadores e calcula seu score de 0 a 100. Quanto melhor for o seu escore mais CoinSaúde você pode ganhar.</p>
          </div>
          <div>
            <h3 className="text-xl font-semibold mb-2">3. Ganhe CoinSaúde</h3>
            <p className="text-gray-600">Melhore sua saúde e acumule moedas digitais para trocar por benefícios reais.</p>
          </div>
        </div>
      </section>
      {/* Para Usuários */}
      <section id="usuario" className="py-20 px-6 bg-gray-50">
        <h2 className="text-3xl font-semibold text-center mb-10">Para Usuários</h2>
        <ul className="max-w-3xl mx-auto space-y-4 text-lg text-gray-700">
          <li>• Score Mérito baseado em exames reais</li>
          <li>• Histórico de saúde organizado e seguro</li>
          <li>• Ganhe CoinSaúde conforme seus resultados</li>
          <li>• Use benefícios em parceiros da saúde e bem-estar</li>
        </ul>
      </section>
      {/* Para Laboratórios */}
      <section id="laboratorio" className="py-20 px-6 bg-white text-center">
        <h2 className="text-3xl font-semibold mb-6">Para Laboratórios</h2>
        <p className="max-w-2xl mx-auto text-gray-700 mb-6">
          A Mérito Autocuidado aumenta a frequência de check-ups, gera engajamento
          e oferece insights agregados para apoiar decisões estratégicas.
        </p>
        <a href="mailto:contato@meritoautocuidado.com.br" className="px-6 py-3 bg-blue-600 text-white rounded-xl font-medium">
          Quero Ser Parceiro
        </a>
      </section>

      {/* Rodapé */}
      <footer className="py-10 text-center text-gray-500 border-t mt-20">
        © 2025 Mérito Autocuidado — Todos os direitos reservados.
      </footer>
    </main>
  );
}
