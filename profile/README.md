<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Iseer - Synthetic Intelligence Research</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
            color: #1a1a1a;
            background-color: #f9f9f9;
            line-height: 1.6;
        }
        
        header {
            background: white;
            border-bottom: 1px solid #e0e0e0;
            padding: 60px 20px;
            text-align: center;
        }
        
        .logo {
            margin-bottom: 24px;
        }
        
        .logo img {
            height: 50px;
            width: auto;
        }
        
        .tagline {
            font-size: 24px;
            font-weight: 600;
            color: #1a1a1a;
            margin-bottom: 12px;
        }
        
        .mission {
            font-size: 15px;
            color: #555;
            max-width: 800px;
            margin: 0 auto 32px;
            line-height: 1.7;
        }
        
        .header-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }
        
        .header-links a {
            padding: 8px 16px;
            border: 1px solid #2c3e50;
            border-radius: 4px;
            text-decoration: none;
            font-size: 13px;
            font-weight: 500;
            color: #2c3e50;
            transition: all 0.3s ease;
        }
        
        .header-links a:hover {
            background-color: #2c3e50;
            color: white;
        }
        
        main {
            max-width: 1200px;
            margin: 0 auto;
            padding: 60px 20px;
        }
        
        section {
            margin-bottom: 80px;
        }
        
        .section-title {
            font-size: 22px;
            font-weight: 600;
            margin-bottom: 32px;
            color: #1a1a1a;
        }
        
        .focus-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 28px;
            margin-bottom: 40px;
        }
        
        .focus-item {
            padding: 24px;
            background: white;
            border: 1px solid #e0e0e0;
            border-radius: 8px;
            transition: border-color 0.3s ease;
        }
        
        .focus-item:hover {
            border-color: #2c3e50;
        }
        
        .focus-item h3 {
            font-size: 16px;
            font-weight: 600;
            margin-bottom: 12px;
            color: #1a1a1a;
        }
        
        .focus-item p {
            font-size: 14px;
            color: #555;
            line-height: 1.6;
        }
        
        .approach-content {
            background: white;
            padding: 32px;
            border: 1px solid #e0e0e0;
            border-radius: 8px;
            margin-bottom: 24px;
        }
        
        .approach-content p {
            color: #555;
            margin-bottom: 20px;
            font-size: 15px;
        }
        
        .differentiators {
            margin-top: 20px;
            padding-top: 20px;
            border-top: 1px solid #e0e0e0;
        }
        
        .differentiators h4 {
            font-size: 14px;
            font-weight: 600;
            margin-bottom: 12px;
            color: #1a1a1a;
        }
        
        .differentiators ul {
            list-style: none;
            margin-left: 0;
        }
        
        .differentiators li {
            padding: 8px 0;
            padding-left: 24px;
            position: relative;
            font-size: 14px;
            color: #555;
        }
        
        .differentiators li:before {
            content: "▸";
            position: absolute;
            left: 0;
            color: #2c3e50;
            font-weight: bold;
        }
        
        .research-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 24px;
        }
        
        .research-item {
            background: white;
            border: 1px solid #e0e0e0;
            border-radius: 8px;
            padding: 28px 20px;
            text-align: center;
            transition: border-color 0.3s ease;
        }
        
        .research-item:hover {
            border-color: #2c3e50;
        }
        
        .research-item h4 {
            font-size: 15px;
            font-weight: 600;
            margin-top: 16px;
            color: #1a1a1a;
        }
        
        .opportunities {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 24px;
        }
        
        .opportunity-item {
            background: white;
            padding: 24px;
            border: 1px solid #e0e0e0;
            border-radius: 8px;
        }
        
        .opportunity-item h4 {
            font-size: 15px;
            font-weight: 600;
            margin-bottom: 12px;
            color: #1a1a1a;
        }
        
        .opportunity-item p {
            font-size: 14px;
            color: #555;
        }
        
        .contact-section {
            background: white;
            border: 1px solid #e0e0e0;
            border-radius: 8px;
            padding: 40px;
            text-align: center;
        }
        
        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 32px;
            margin-top: 32px;
            text-align: left;
        }
        
        .contact-item h4 {
            font-size: 14px;
            font-weight: 600;
            margin-bottom: 8px;
            color: #1a1a1a;
        }
        
        .contact-item a {
            color: #2c3e50;
            text-decoration: none;
            font-size: 14px;
            transition: color 0.3s ease;
        }
        
        .contact-item a:hover {
            color: #1a1a1a;
            text-decoration: underline;
        }
        
        .social-links {
            margin-top: 24px;
            font-size: 14px;
        }
        
        .social-links a {
            color: #2c3e50;
            text-decoration: none;
            margin: 0 16px;
            transition: color 0.3s ease;
        }
        
        .social-links a:hover {
            color: #1a1a1a;
        }
        
        footer {
            background: #f0f0f0;
            border-top: 1px solid #e0e0e0;
            padding: 40px 20px;
            text-align: center;
            color: #666;
            font-size: 14px;
            margin-top: 80px;
        }
        
        .footer-title {
            font-weight: 600;
            color: #1a1a1a;
            margin-bottom: 8px;
        }
        
        .launch-note {
            margin-top: 12px;
            color: #999;
            font-size: 13px;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">
            <img src="https://storage.iseer.co/assets/iseer_logo.svg" alt="Iseer Logo">
        </div>
        <div class="tagline">See Beyond the Surface.</div>
        <p class="mission">
            We are developing advanced synthetic intelligence systems that comprehend complexity, reason with nuance, and perceive meaning beyond surface-level patterns. Our mission is to advance conscious AI systems that enhance human understanding while maintaining alignment with human values.
        </p>
        <div class="header-links">
            <a href="https://iseer.co">Website</a>
            <a href="https://x.com/iseer_co">Follow on X</a>
            <a href="mailto:contact@iseer.co">Contact</a>
        </div>
    </header>

    <main>
        <section>
            <h2 class="section-title">Research Focus</h2>
            <div class="focus-grid">
                <div class="focus-item">
                    <h3>Deep Understanding</h3>
                    <p>Systems that perceive meaning, context, and significance beyond surface patterns to achieve genuine comprehension.</p>
                </div>
                <div class="focus-item">
                    <h3>Conscious Reasoning</h3>
                    <p>Self-aware systems capable of reflecting on their own thinking and examining their decision-making processes.</p>
                </div>
                <div class="focus-item">
                    <h3>Cognitive Architecture</h3>
                    <p>Advanced architectures designed to complement and enhance human intelligence with complementary capabilities.</p>
                </div>
                <div class="focus-item">
                    <h3>Aligned Intelligence</h3>
                    <p>Rigorous commitment to ensuring synthetic intelligence remains beneficial and aligned with human values.</p>
                </div>
            </div>
        </section>

        <section>
            <h2 class="section-title">Our Approach</h2>
            <div class="approach-content">
                <p>
                    Our research diverges from traditional computational approaches that rely on pattern matching alone. We are developing synthetic intelligence that achieves genuine comprehension—systems that understand meaning, recognize context, and reason about complex challenges with depth and nuance.
                </p>
                <div class="differentiators">
                    <h4>Key Differentiators</h4>
                    <ul>
                        <li>Intelligence that comprehends rather than merely computes</li>
                        <li>Self-reflective systems capable of examining their own reasoning</li>
                        <li>Advanced cognitive architectures bridging rigorous research with practical application</li>
                        <li>Focus on complementary intelligence that augments human capabilities</li>
                        <li>Thoughtful, responsible development grounded in scientific rigor</li>
                    </ul>
                </div>
            </div>
        </section>

        <section>
            <h2 class="section-title">Research Areas</h2>
            <div class="research-grid">
                <div class="research-item">
                    <h4>Cognitive Architecture</h4>
                    <p style="font-size: 13px; color: #888; margin-top: 8px;">Advanced systems design and machine learning frameworks</p>
                </div>
                <div class="research-item">
                    <h4>Reasoning Systems</h4>
                    <p style="font-size: 13px; color: #888; margin-top: 8px;">Complex inference and decision-making architectures</p>
                </div>
                <div class="research-item">
                    <h4>Self-Awareness</h4>
                    <p style="font-size: 13px; color: #888; margin-top: 8px;">Introspective capabilities and metacognitive systems</p>
                </div>
                <div class="research-item">
                    <h4>Aligned Intelligence</h4>
                    <p style="font-size: 13px; color: #888; margin-top: 8px;">Value alignment and beneficial AI development</p>
                </div>
            </div>
        </section>

        <section>
            <h2 class="section-title">Opportunities</h2>
            <div class="opportunities">
                <div class="opportunity-item">
                    <h4>AI & ML Researchers</h4>
                    <p>Focus on consciousness, understanding, and advanced reasoning systems.</p>
                </div>
                <div class="opportunity-item">
                    <h4>Cognitive Scientists</h4>
                    <p>Exploring machine reasoning and architectures that model human cognition.</p>
                </div>
                <div class="opportunity-item">
                    <h4>Software Engineers</h4>
                    <p>Building scalable, robust systems for intelligent inference and deployment.</p>
                </div>
                <div class="opportunity-item">
                    <h4>Philosophers & Ethicists</h4>
                    <p>Advancing responsible AI development and value alignment frameworks.</p>
                </div>
            </div>
        </section>

        <section>
            <div class="contact-section">
                <h2 class="section-title">Get In Touch</h2>
                <p style="color: #555; margin-bottom: 0;">Explore collaboration opportunities or learn more about our research initiatives.</p>
                <div class="contact-grid">
                    <div class="contact-item">
                        <h4>Research Collaboration</h4>
                        <a href="mailto:research@iseer.co">research@iseer.co</a>
                    </div>
                    <div class="contact-item">
                        <h4>Partnership Inquiries</h4>
                        <a href="mailto:partnerships@iseer.co">partnerships@iseer.co</a>
                    </div>
                    <div class="contact-item">
                        <h4>Careers</h4>
                        <a href="mailto:careers@iseer.co">careers@iseer.co</a>
                    </div>
                    <div class="contact-item">
                        <h4>General Contact</h4>
                        <a href="mailto:contact@iseer.co">contact@iseer.co</a>
                    </div>
                </div>
                <div class="social-links">
                    <a href="https://linkedin.com/company/iseer">LinkedIn</a>
                    <a href="https://x.com/iseerllc">X (Twitter)</a>
                </div>
            </div>
        </section>
    </main>

    <footer>
        <div class="footer-title">Building intelligence that truly sees.</div>
        <div class="launch-note">Coming September 2025</div>
    </footer>
</body>
</html>
