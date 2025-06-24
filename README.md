    :root {
        --primary-color: #2c3e50;
        --secondary-color: #3498db;
        --accent-color: #e74c3c;
        --light-color: #ecf0f1;
        --dark-color: #2c3e50;
        --transition: all 0.3s ease;
    }
    
    body {
        background: linear-gradient(135deg, #1a2a6c, #b21f1f, #1a2a6c);
        color: var(--light-color);
        line-height: 1.6;
        min-height: 100vh;
        display: flex;
        flex-direction: column;
    }
    
    header {
        background-color: rgba(0, 0, 0, 0.7);
        padding: 1.5rem;
        text-align: center;
        position: relative;
        border-bottom: 3px solid var(--accent-color);
    }
    
    .banner {
        background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), 
                     url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="800" height="200" viewBox="0 0 800 200"><rect width="800" height="200" fill="%232c3e50"/><text x="50%" y="50%" font-family="Arial" font-size="24" fill="%23ecf0f1" text-anchor="middle" dominant-baseline="middle">AL HASSAN TRAVEL & TOURISM</text></svg>');
        background-size: cover;
        background-position: center;
        height: 200px;
        display: flex;
        align-items: center;
        justify-content: center;
        border-radius: 10px;
        margin: 0 auto 2rem;
        box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
    }
    
    .banner h1 {
        font-size: 2.5rem;
        color: white;
        text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.8);
        letter-spacing: 3px;
    }
    
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 2rem;
        flex: 1;
    }
    
    .profile-section {
        background: rgba(44, 62, 80, 0.9);
        border-radius: 15px;
        padding: 2.5rem;
        margin-bottom: 2rem;
        box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        border: 1px solid rgba(255, 255, 255, 0.1);
    }
    
    .profile-header {
        text-align: center;
        margin-bottom: 2rem;
        position: relative;
    }
    
    .profile-header h1 {
        font-size: 2.8rem;
        color: var(--secondary-color);
        margin-bottom: 1rem;
        position: relative;
        display: inline-block;
    }
    
    .profile-header h1::after {
        content: "";
        position: absolute;
        bottom: -10px;
        left: 50%;
        transform: translateX(-50%);
        width: 100px;
        height: 4px;
        background: var(--accent-color);
        border-radius: 2px;
    }
    
    .profile-header h2 {
        font-size: 1.8rem;
        font-weight: 400;
        color: var(--light-color);
        margin-bottom: 1.5rem;
    }
    
    .info-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 1.5rem;
        margin-top: 2rem;
    }
    
    .info-card {
        background: rgba(52, 73, 94, 0.7);
        border-radius: 10px;
        padding: 1.5rem;
        transition: var(--transition);
        border: 1px solid rgba(255, 255, 255, 0.1);
    }
    
    .info-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        background: rgba(52, 73, 94, 0.9);
    }
    
    .info-card h3 {
        color: var(--secondary-color);
        margin-bottom: 1rem;
        font-size: 1.5rem;
        display: flex;
        align-items: center;
    }
    
    .info-card h3 i {
        margin-left: 10px;
        color: var(--accent-color);
    }
    
    .info-card p {
        font-size: 1.1rem;
        margin-bottom: 0.5rem;
    }
    
    .skills-section {
        margin-top: 2rem;
    }
    
    .skills-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        gap: 1rem;
        margin-top: 1.5rem;
    }
    
    .skill-card {
        background: rgba(52, 152, 219, 0.2);
        border-radius: 8px;
        padding: 1.2rem;
        text-align: center;
        transition: var(--transition);
        border: 1px solid rgba(255, 255, 255, 0.1);
    }
    
    .skill-card:hover {
        background: rgba(52, 152, 219, 0.4);
        transform: scale(1.05);
    }
    
    .skill-card i {
        font-size: 2.5rem;
        color: var(--secondary-color);
        margin-bottom: 1rem;
    }
    
    .university-link {
        display: block;
        text-align: center;
        margin: 2.5rem 0;
    }
    
    .university-link a {
        display: inline-block;
        background: linear-gradient(to right, var(--accent-color), #c0392b);
        color: white;
        text-decoration: none;
        font-size: 1.5rem;
        font-weight: bold;
        padding: 1rem 3rem;
        border-radius: 50px;
        transition: var(--transition);
        box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        border: none;
        position: relative;
        overflow: hidden;
    }
    
    .university-link a:hover {
        transform: translateY(-5px);
        box-shadow: 0 10px 25px rgba(231, 76, 60, 0.4);
    }
    
    .university-link a::before {
        content: "";
        position: absolute;
        top: 0;
        left: -100%;
        width: 100%;
        height: 100%;
        background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
        transition: 0.5s;
    }
    
    .university-link a:hover::before {
        left: 100%;
    }
    
    footer {
        background: rgba(0, 0, 0, 0.8);
        text-align: center;
        padding: 1.5rem;
        margin-top: 2rem;
        border-top: 1px solid rgba(255, 255, 255, 0.1);
    }
    
    .university-page {
        display: none;
    }
    
    .back-link {
        display: block;
        text-align: center;
        margin-top: 2rem;
    }
    
    .back-link a {
        color: var(--secondary-color);
        text-decoration: none;
        font-size: 1.2rem;
        display: inline-flex;
        align-items: center;
        transition: var(--transition);
    }
    
    .back-link a:hover {
        color: var(--accent-color);
        transform: translateX(-5px);
    }
    
    .university-logo {
        text-align: center;
        margin: 2rem 0;
    }
    
    .university-logo .logo {
        width: 150px;
        height: 150px;
        background: linear-gradient(45deg, var(--secondary-color), var(--primary-color));
        border-radius: 50%;
        display: inline-flex;
        align-items: center;
        justify-content: center;
        font-size: 2.5rem;
        color: white;
        box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        border: 3px solid var(--accent-color);
    }
    
    .study-details {
        background: rgba(44, 62, 80, 0.9);
        border-radius: 15px;
        padding: 2.5rem;
        margin: 2rem 0;
        box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        border: 1px solid rgba(255, 255, 255, 0.1);
    }
    
    .study-details h2 {
        text-align: center;
        color: var(--secondary-color);
        margin-bottom: 2rem;
        font-size: 2rem;
        position: relative;
    }
    
    .study-details h2::after {
        content: "";
        position: absolute;
        bottom: -10px;
        left: 50%;
        transform: translateX(-50%);
        width: 80px;
        height: 4px;
        background: var(--accent-color);
        border-radius: 2px;
    }
    
    .details-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        gap: 1.5rem;
        margin-top: 2rem;
    }
    
    .detail-card {
        background: rgba(52, 73, 94, 0.7);
        border-radius: 10px;
        padding: 1.5rem;
        text-align: center;
        transition: var(--transition);
        border: 1px solid rgba(255, 255, 255, 0.1);
    }
    
    .detail-card:hover {
        transform: translateY(-5px);
        background: rgba(52, 73, 94, 0.9);
    }
    
    .detail-card h3 {
        ...
