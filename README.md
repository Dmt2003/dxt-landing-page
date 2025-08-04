[package.json](https://github.com/user-attachments/files/21578290/package.json)
{
  "name": "dxt-landing-page",
  "version": "1.0.0",
  "private": true,
  "dependencies": {
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "react-scripts": "5.0.1"
  },
  "scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",[Uploading index.html…<!DOCTYPE html><html lang="pt-br"><head><meta charset="UTF-8" /><meta name="viewport" content="width=device-width, initial-scale=1.0" /><title>DXT Soluções</title></head><body><div id="root"></div></body></html>]()

    "test": "react-scripts test",
    "eject": "react-scripts eject"
  }
}
import React from "react";

export default function Home() {
  return (
    <div className="bg-gray-100 text-gray-800">
      <section className="bg-black text-white py-20 px-6 text-center bg-cover bg-center" style={{ backgroundImage: "url('/assets/hero-bg.jpg')" }}>
        <img src="/assets/DXT_Logo_Final_v01.jpg" alt="Logo DXT" className="mx-auto mb-6 h-16 md:h-20" />
        <h1 className="text-4xl md:text-5xl font-bold mb-6">Tecnologia e Segurança 24h</h1>
        <p className="text-xl mb-8">Proteção inteligente para sua casa, empresa ou condomínio.</p>
        <div className="flex justify-center gap-4">
          <a href="#servicos" className="bg-blue-600 px-6 py-3 rounded-xl hover:bg-blue-700 transition">Conheça nossos serviços</a>
          <a href="https://wa.me/5511985159327" target="_blank" rel="noopener noreferrer" className="border border-white px-6 py-3 rounded-xl hover:bg-white hover:text-black transition">Fale no WhatsApp</a>
        </div>
      </section>![DXT_Logo_Final_v01](https://github.com/user-attachments/assets/2a38f739-5ac9-4d66-a035-7be9e021898e)

      <section className="py-16 px-6 bg-white text-center">
        <h2 className="text-3xl font-bold mb-6">Conheça a DXT</h2>
        <div className="aspect-w-16 aspect-h-9 max-w-4xl mx-auto">
          <video controls className="rounded-xl shadow-md">
            <source src="/assets/video-institucional.mp4" type="video/mp4" />
            Seu navegador não suporta vídeo.
          </video>
        </div>
      </section>

      <section className="py-16 px-6 max-w-5xl mx-auto" id="sobre">
        <h2 className="text-3xl font-bold mb-6">Sobre a DXT</h2>
        <p className="mb-4">A DXT é uma empresa de segurança eletrônica focada em tecnologias para proteger seu patrimônio. Nossa missão é fornecer soluções inovadoras com ética, transparência e qualidade.</p>
        <ul className="list-disc pl-6 space-y-2">
          <li><strong>Missão:</strong> Fornecer soluções inovadoras e serviços de segurança individualizados</li>
          <li><strong>Visão:</strong> Ser referência em excelência no mercado cearense</li>
          <li><strong>Valores:</strong> Ética, inovação, excelência e respeito</li>
        </ul>
      </section>
    </div>
  );
}

import React from "react"; import ReactDOM from "react-dom/client"; import Home from "./Home"; import './style.css'; const root = ReactDOM.createRoot(document.getElementById("root")); root.render(<Home />);
body { margin: 0; font-family: sans-serif; }
