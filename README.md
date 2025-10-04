<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>My Game Zone 🎮</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap');
    * {
      box-sizing: border-box;
    }
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: radial-gradient(circle at top, #0f172a, #020617);
      color: #e2e8f0;
      display: flex;
      flex-direction: column;
      min-height: 100vh;
    }

    /* Navbar */
    nav {
      background: rgba(255,255,255,0.05);
      border-bottom: 1px solid rgba(255,255,255,0.1);
      backdrop-filter: blur(10px);
      position: sticky;
      top: 0;
      z-index: 10;
    }
    .nav-container {
      max-width: 1100px;
      margin: 0 auto;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 12px 20px;
    }
    .logo {
      font-weight: 700;
      font-size: 1.4rem;
      color: #38bdf8;
      cursor: pointer;
    }
    .menu {
      display: flex;
      gap: 24px;
    }
    .menu a {
      color: #e2e8f0;
      text-decoration: none;
      font-weight: 500;
      transition: 0.2s;
    }
    .menu a:hover {
      color: #22d3ee;
    }

    /* Hero Section */
    header {
      text-align: center;
      margin-top: 60px;
    }
    h1 {
      font-size: 2.6rem;
      color: #38bdf8;
    }
    p.subtitle {
      color: #94a3b8;
      font-size: 1.1rem;
      margin-top: 8px;
    }

    /* Game Grid */
    .games {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      gap: 24px;
      width: 90%;
      max-width: 1000px;
      margin: 50px auto;
    }
    .card {
      background: rgba(255,255,255,0.05);
      border: 2px solid rgba(255,255,255,0.08);
      border-radius: 16px;
      overflow: hidden;
      text-align: center;
      transition: 0.3s ease;
      box-shadow: 0 8px 20px rgba(0,0,0,0.4);
      position: relative;
    }
    .card:hover {
      transform: translateY(-8px) scale(1.03);
      border-color: #22d3ee;
      background: rgba(255,255,255,0.08);
    }
    .card img {
      width: 100%;
      height: 150px;
      object-fit: cover;
      border-bottom: 1px solid rgba(255,255,255,0.08);
    }
    .card-content {
      padding: 16px;
    }
    .card h2 {
      margin: 8px 0;
      color: #e0f2fe;
      font-size: 1.2rem;
    }
    .card p {
      color: #94a3b8;
      font-size: 0.9rem;
      margin-bottom: 16px;
    }
    .card button {
      background: #22d3ee;
      color: #0f172a;
      border: none;
      border-radius: 10px;
      padding: 10px 18px;
      cursor: pointer;
      font-weight: 600;
      transition: 0.2s;
    }
    .card button:hover {
      background: #06b6d4;
    }

    /* About Section */
    section.about {
      max-width: 800px;
      margin: 60px auto;
      text-align: center;
      color: #cbd5e1;
      line-height: 1.6;
      background: rgba(255,255,255,0.03);
      padding: 30px;
      border-radius: 14px;
    }

    footer {
      text-align: center;
