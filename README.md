# 🕹️ Máquina Pegadora (Claw Machine)

Uma simulação interativa de uma **Máquina Pegadora** (ou "Claw Machine") construída puramente com **HTML5**, **CSS3** (com ênfase em Pixels/Estilo Retrô) e **JavaScript**.

O projeto foca em recriar a experiência clássica do jogo de arcade, utilizando a manipulação do DOM e a estilização detalhada para dar vida aos componentes da máquina e suas interações.

---

## ✨ Funcionalidades

* **Controles Interativos:** Botões funcionais para mover o braço da máquina horizontalmente e verticalmente.
* **Estilo Retrô (Pixel Art):** Uso da classe `.pix` e estilização CSS para simular um visual de pixel art e retrô.
* **Estrutura da Máquina:** Componentes visuais detalhados, como o trilho, o braço articulado, as garras e a área de coleta.
* **Animação Simples (via JS):** O JavaScript manipula as propriedades CSS (provavelmente `transform: translate()` ou `position`) para simular o movimento das garras.

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Descrição |
| :--- | :--- |
| **HTML5** | Estrutura semântica e hierarquia dos componentes da máquina. |
| **CSS3** | Estilização completa, incluindo layout, cores e o estilo **Pixel Art/Retrô**. |
| **JavaScript (ES6+)** | Lógica de controle dos botões e a movimentação do braço da máquina (manipulação de classes e estilos). |

---

## ⚙️ Estrutura do Código (Visão Geral)

O HTML utiliza classes claras para representar cada parte física da máquina, facilitando a estilização e a manipulação via JavaScript.

### Estrutura HTML (`index.html`)

A estrutura central está dentro do container `.claw-machine`.

```html
<div class="claw-machine">
  <div class="box pix">
    <div class="machine-top pix">
      <div class="arm-joint pix">
        <div class="arm pix">
          <div class="claws pix"></div>
        </div>
      </div>
      <div class="rail hori pix"></div>
      <div class="rail vert pix"></div>
    </div>

    <div class="machine-bottom pix">...</div>
  </div>

  <div class="control pix">
    <button class="hori-btn pix"></button>
    <button class="vert-btn pix"></button>
    </div>
</div>
