<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Volupta® - A cinta que veste sua confiança. Modeladora 360º com compressão confortável. Compre 1, Leve 2!">
    <meta name="theme-color" content="#E91E63">
    <title>Volupta® | A cinta que veste sua confiança</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700;800&display=swap" rel="stylesheet">
</head>
<body>
    <!-- ===== HEADER BANNER ===== -->
    <header class="banner-promo">
        <p>🚚 FRETE GRÁTIS PARA TODO O BRASIL · OFERTA ESPECIAL POR TEMPO LIMITADO</p>
    </header>

    <!-- ===== NAVBAR ===== -->
    <nav class="navbar">
        <div class="nav-container">
            <div class="logo">VOLUPTA®</div>
            <div class="nav-links">
                <a href="#about">Sobre</a>
                <a href="#benefits">Benefícios</a>
                <a href="#reviews">Avaliações</a>
                <a href="#contact">Contato</a>
            </div>
        </div>
    </nav>

    <!-- ===== HERO SECTION ===== -->
    <section class="hero">
        <div class="hero-content">
            <div class="hero-text">
                <h1>Modeladora Volupta®</h1>
                <p class="subtitle">Compre 1, Leve 2</p>
                <p class="hero-description">Modelagem 360º para barriga, cintura e costas, com compressão confortável para acompanhar sua rotina.</p>
                
                <div class="hero-badges">
                    <span class="badge">⭐ 4,8/5 Avaliações verificadas</span>
                    <span class="badge">🏆 Mais vendida</span>
                    <span class="badge">🚚 Envio nacional</span>
                    <span class="badge">✓ Garantia de 60 dias</span>
                </div>

                <div class="price-section">
                    <div class="discount-badge">57% OFF</div>
                    <div class="price-container">
                        <span class="price-old">R$ 299,80</span>
                        <span class="price-current">R$ 129,90</span>
                        <span class="price-method">no Pix</span>
                    </div>
                    <p class="price-info">ou R$ 159,90 no cartão ou boleto · até 12x de R$ 13,33</p>
                </div>

                <a href="#purchase" class="btn-primary">COMPRAR AGORA</a>
            </div>

            <div class="hero-images">
                <img src="images/modeladora-preto.jpg" alt="Modeladora Volupta® preta">
                <img src="images/modeladora-bege.jpg" alt="Modeladora Volupta® bege">
            </div>
        </div>
    </section>

    <!-- ===== PURCHASE SECTION ===== -->
    <section id="purchase" class="purchase-section">
        <div class="purchase-container">
            <h2>Escolha sua combinação</h2>
            
            <div class="offer-box">
                <img src="images/oferta-aniversario.jpg" alt="Oferta Compre 1 Leve 2" class="offer-image">
                
                <div class="combo-options">
                    <div class="combo-option" data-combo="bege-preto">
                        <input type="radio" id="combo1" name="combo" value="bege-preto" checked>
                        <label for="combo1">
                            <div class="color-preview">
                                <div class="color-bege"></div>
                                <div class="color-preto"></div>
                            </div>
                            <span>Bege + Preto</span>
                        </label>
                    </div>

                    <div class="combo-option" data-combo="bege-bege">
                        <input type="radio" id="combo2" name="combo" value="bege-bege">
                        <label for="combo2">
                            <div class="color-preview">
                                <div class="color-bege"></div>
                                <div class="color-bege"></div>
                            </div>
                            <span>Bege + Bege</span>
                        </label>
                    </div>

                    <div class="combo-option" data-combo="preto-preto">
                        <input type="radio" id="combo3" name="combo" value="preto-preto">
                        <label for="combo3">
                            <div class="color-preview">
                                <div class="color-preto"></div>
                                <div class="color-preto"></div>
                            </div>
                            <span>Preto + Preto</span>
                        </label>
                    </div>
                </div>

                <div class="size-section">
                    <h3>Escolha seu tamanho</h3>
                    <div class="size-options">
                        <label class="size-option">
                            <input type="radio" name="size" value="P" checked>
                            <span>P</span>
                        </label>
                        <label class="size-option">
                            <input type="radio" name="size" value="M">
                            <span>M</span>
                        </label>
                        <label class="size-option">
                            <input type="radio" name="size" value="G">
                            <span>G</span>
                        </label>
                        <label class="size-option">
                            <input type="radio" name="size" value="GG">
                            <span>GG</span>
                        </label>
                    </div>
                    <a href="#" class="size-guide">Qual é o meu tamanho?</a>
                </div>

                <div class="shipping-info">
                    <p><strong>📦 Envio Nacional</strong> · Frete grátis para todo o Brasil</p>
                </div>

                <button class="btn-primary btn-large">COMPRAR AGORA</button>

                <div class="trust-badges">
                    <div class="trust-badge">✓ Compra segura</div>
                    <div class="trust-badge">🔒 Pagamento protegido</div>
                    <div class="trust-badge">🚚 Envio para todo o Brasil</div>
                    <div class="trust-badge">↩️ Devolução gratuita</div>
                    <div class="trust-badge">⏱️ 60 dias de garantia</div>
                </div>
            </div>
        </div>
    </section>

    <!-- ===== BENEFITS SECTION ===== -->
    <section id="benefits" class="benefits">
        <h2>Uma peça. Quatro benefícios.</h2>
        <div class="benefits-grid">
            <div class="benefit-card">
                <div class="benefit-icon">🔄</div>
                <h3>Compressão 360º</h3>
                <p>Modela barriga, cintura e costas de forma uniforme.</p>
            </div>

            <div class="benefit-card">
                <div class="benefit-icon">💪</div>
                <h3>Mais firmeza</h3>
                <p>A estrutura ajuda a manter a peça posicionada durante o uso.</p>
            </div>

            <div class="benefit-card">
                <div class="benefit-icon">☁️</div>
                <h3>Conforto</h3>
                <p>Tecido pensado para acompanhar a rotina sem sensação excessiva de aperto.</p>
            </div>

            <div class="benefit-card">
                <div class="benefit-icon">✨</div>
                <h3>Silhueta valorizada</h3>
                <p>Ajuda a criar uma aparência mais uniforme sob diferentes tipos de roupa.</p>
            </div>
        </div>
    </section>

    <!-- ===== BEFORE & AFTER ===== -->
    <section class="before-after">
        <h2>Veja a diferença no caimento.</h2>
        <p class="subtitle-section">Uma modeladora pensada para vestir melhor, sem transformar seu corpo em outra pessoa.</p>
        
        <div class="before-after-container">
            <div class="comparison-item">
                <img src="images/antes-depois-frente.jpg" alt="Comparação frente">
                <p><strong>Frente</strong> — caimento mais uniforme na cintura e barriga.</p>
            </div>
            <div class="comparison-item">
                <img src="images/antes-depois-costas.jpg" alt="Comparação costas">
                <p><strong>Costas</strong> — menos marcas sob a roupa.</p>
            </div>
        </div>
        <p class="disclaimer">Imagens de uso com peça vestida. Resultados de caimento variam conforme corpo, tamanho e roupa.</p>
    </section>

    <!-- ===== HOW IT WORKS ===== -->
    <section class="how-it-works">
        <h2>Como funciona</h2>
        <div class="steps-container">
            <div class="step">
                <div class="step-number">01</div>
                <h3>Vista</h3>
                <p>Suba a peça até a cintura alta, sem dobrar o cós.</p>
            </div>

            <div class="step-arrow">→</div>

            <div class="step">
                <div class="step-number">02</div>
                <h3>Ajuste</h3>
                <p>Alinhe as laterais e acomode o tecido no corpo.</p>
            </div>

            <div class="step-arrow">→</div>

            <div class="step">
                <div class="step-number">03</div>
                <h3>Siga o dia</h3>
                <p>Vista sua roupa e siga o dia com liberdade.</p>
            </div>
        </div>
    </section>

    <!-- ===== REVIEWS SECTION ===== -->
    <section id="reviews" class="reviews">
        <h2>Quem ama Volupta ⭐</h2>
        <p class="subtitle-section">Experiências de mulheres que escolheram a Volupta para acompanhar sua rotina.</p>

        <div class="stats-container">
            <div class="stat">
                <div class="stat-number">2.847</div>
                <div class="stat-label">Avaliações verificadas</div>
            </div>
            <div class="stat">
                <div class="stat-number">18.932</div>
                <div class="stat-label">Peças enviadas</div>
            </div>
            <div class="stat">
                <div class="stat-number">4,8/5</div>
                <div class="stat-label">Nota média</div>
            </div>
        </div>

        <div class="reviews-carousel">
            <div class="review-card">
                <div class="review-header">
                    <div class="review-avatar">MA</div>
                    <div class="review-info">
                        <strong>Mariana Alves</strong>
                        <p>São Paulo — SP</p>
                    </div>
                    <div class="review-rating">⭐⭐⭐⭐⭐</div>
                </div>
                <p class="review-text">"Gostei muito da modelagem. A peça ficou bem ajustada no meu corpo e por baixo da roupa praticamente não aparece. O que mais gostei foi poder usar durante o dia sem ficar pensando nela o tempo todo."</p>
                <p class="verified">✓ Comentário verificado pelo Google</p>
            </div>

            <div class="review-card">
                <div class="review-header">
                    <div class="review-avatar">CR</div>
                    <div class="review-info">
                        <strong>Camila Rodrigues</strong>
                        <p>Belo Horizonte — MG</p>
                    </div>
                    <div class="review-rating">⭐⭐⭐⭐⭐</div>
                </div>
                <p class="review-text">"Foi a primeira cinta que comprei e fiquei surpresa com o caimento. Escolhi meu tamanho seguindo o guia e ficou bem confortável. Principalmente com vestidos e roupas mais justas, gostei bastante do resultado."</p>
                <p class="verified">✓ Comentário verificado pelo Google</p>
            </div>

            <div class="review-card">
                <div class="review-header">
                    <div class="review-avatar">JM</div>
                    <div class="review-info">
                        <strong>Juliana Martins</strong>
                        <p>Rio de Janeiro — RJ</p>
                    </div>
                    <div class="review-rating">⭐⭐⭐⭐⭐</div>
                </div>
                <p class="review-text">"Comprei a combinação preta e bege e achei muito prática. A preta virou minha favorita para usar com roupas escuras. Gostei bastante da firmeza e do acabamento."</p>
                <p class="verified">✓ Comentário verificado pelo Google</p>
            </div>

            <div class="review-card">
                <div class="review-header">
                    <div class="review-avatar">FO</div>
                    <div class="review-info">
                        <strong>Fernanda Oliveira</strong>
                        <p>Curitiba — PR</p>
                    </div>
                    <div class="review-rating">⭐⭐⭐⭐⭐</div>
                </div>
                <p class="review-text">"O que mais me chamou atenção foi que ela fica bem posicionada enquanto estou sentada ou andando. Para mim isso fez bastante diferença em comparação com outras peças que já tinha usado."</p>
                <p class="verified">✓ Comentário verificado pelo Google</p>
            </div>

            <div class="review-card">
                <div class="review-header">
                    <div class="review-avatar">AS</div>
                    <div class="review-info">
                        <strong>Aline Santos</strong>
                        <p>Salvador — BA</p>
                    </div>
                    <div class="review-rating">⭐⭐⭐⭐⭐</div>
                </div>
                <p class="review-text">"Adorei a experiência. A peça deixa a roupa com um caimento muito mais bonito e me senti bem mais confiante usando algumas roupas que estavam paradas no armário."</p>
                <p class="verified">✓ Comentário verificado pelo Google</p>
            </div>

            <div class="review-card">
                <div class="review-header">
                    <div class="review-avatar">PC</div>
                    <div class="review-info">
                        <strong>Patrícia Costa</strong>
                        <p>Brasília — DF</p>
                    </div>
                    <div class="review-rating">⭐⭐⭐⭐⭐</div>
                
