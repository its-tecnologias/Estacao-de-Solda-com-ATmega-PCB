# Alerta! ⚠️
Se você está usando a versão com "t", saiba que ela é uma versão de teste! Pode haver problemas de estabilidade, e não é recomendado para ambientes de produção. Não diga que eu não avisei! 😅

## Visão Geral 🌟

**T12: A Estação de Solda Rápida da iTS Tecnologias, desenvolvida pelo Michel Menezes da Silva**

Aqui na iTS Tecnologias, não fazemos uma simples estação de solda. A nossa T12 é um controlador poderoso que pode fazer praticamente tudo, menos soldar sozinha (ainda). Vem com:

- **Monitoramento em tempo real da temperatura da ponta** – Para garantir que está tudo no ponto certo, sem surpresas!
- **Controle PID de temperatura** – Para aqueles que gostam de precisão. Ou controle direto, se você for old school.
- **Controle de temperatura via encoder** – Gire para ajustar, simples assim.
- **Modo turbo (boost)** – Precisa de um calor extra rápido? Um clique curto no encoder e boom! Modo turbo ativado!
- **Menu de configurações** – Com um toque longo no encoder, você abre o menu principal e ajusta tudo ao seu gosto.
- **Detecção de movimento no cabo (se tiver um sensor de movimento)** – Porque sabemos que você não quer que a solda esfrie se estiver só fazendo uma pausa.
- **Detecção de desconexão do cabo de solda** – Ninguém gosta de surpresas, especialmente quando a ponta da solda não está conectada.
- **Modo sleep e desligamento automático** – Para economizar energia e estender a vida útil do seu equipamento quando você não está soldando.
- **Monitoramento da voltagem e temperatura interna** – Só para garantir que está tudo funcionando perfeitamente.
- **Display OLED** – Quem disse que uma estação de solda não pode ter estilo?
- **Buzzer** – Sim, tem um apito para te avisar quando algo não está certo.
- **Calibração de diferentes pontas de solda** – Porque cada ponta tem suas manhas.
- **Configurações salvas na EEPROM** – Acabou a energia? Sem problemas! As configurações estão guardadas.
- **Detecção de troca de ponta de solda** – A estação é inteligente o suficiente para reconhecer quando você trocou a ponta e até abre o menu de seleção.
- **Suporte para MOSFETs N-Channel e P-Channel** – Flexibilidade é o nome do jogo!

## Versão UI Melhorada 🚀

A iTS Tecnologias sempre está atualizando as coisas para que você tenha a melhor experiência possível!

- **Alerta de superaquecimento e baixa tensão** – Segurança primeiro, sempre!
- **Barras de temperatura e potência em tempo real** – Para você acompanhar tudo visualmente.
- **Animações de transição** – Porque quem não ama uma boa animação, certo?
- **Protetor de tela embutido** – Para manter o OLED saudável e estiloso.
- **Opção de virar a tela** – Se você está virando a estação, a tela acompanha.
- **Suporte para inglês e chinês** – Poliglota sim, senhor!
- **Senha de proteção ao iniciar** – Segurança extra para evitar acidentes.
- **Ajuste da direção do botão** – Para quem gosta de personalizar tudo.
- **Watchdog** – Se o sistema travar (o que é raro, mas acontece), ele reinicia automaticamente. Prático, não é?

## Novidades da V1.8t7 🎉

- **Verificação da EEPROM** – Ninguém merece uma EEPROM bugada, né? Agora tem uma checagem automática!
- **Suporte para até 30 pontas de solda diferentes** – Para quem leva a diversidade a sério.
- **Curva de temperatura com 9 segmentos** – Mais controle, mais precisão!

## Links Úteis 🔗

- Vídeo do projeto: [Aqui no YouTube](https://youtu.be/I9ATDxvQ1Bc)
- Vídeo de John Glavinos: [Assista aqui](https://youtu.be/4YDcWfOQmz4)
- Vídeo da UI por LHW-createskyblue: [Bilibili - A magia acontece aqui!](https://b23.tv/LiOe54)
- Versão T245 por TaaraLabs: [Confira o trabalho deles](https://taaralabs.eu/atmega-t245/)

## Notas e Observações 📝

Ah, claro! Não somos perfeitos, e há algumas coisinhas que você deve ter em mente. Na versão da placa 2.5, o diodo D1 pode superaquecer. Para garantir que não vire um problema, remova o diodo zener D4 e opere a estação com no máximo 20V. Ou, se preferir, substitua o D1 por um diodo Schottky SS54 e o transistor Q1 por um FMMT619. Seu futuro você escolhe! 💡

## Especificações de Alimentação ⚡

Escolha sua fonte de alimentação com sabedoria, jovem padawan! Use uma fonte com tensão entre 12V e 24V, e siga a tabelinha mágica abaixo para corrente e potência:

| Tensão (V) | Corrente (A) = U / R | Potência (W) = U² / R |
|------------|----------------------|-----------------------|
| 12 V       | 1.50 A               | 18 W                  |
| 24 V       | 3.00 A               | 72 W                  |

Simples, não? Apenas escolha sua fonte de acordo com a resistência de 8 ohms do aquecedor.

## Medição de Temperatura e Considerações sobre o OpAmp 🌡️

A ponta da solda T12 possui um termopar (sensor de temperatura). A medição da temperatura depende de um amplificador operacional (OpAmp). Embora a LMV358 funcione, ela não é o ideal para alta precisão. Recomendamos o OPA2330AIDR para medições mais precisas e estáveis. Vale o investimento!

## Troca Inteligente do MOSFET 🔧

Ao usar MOSFETs de canal N, a eficiência sobe e o calor diminui. No entanto, precisa de um circuito adicional (a famosa bomba de carga) para funcionar corretamente. É isso que usamos para manter tudo sob controle!

## Instruções de Montagem 🛠️

Além dos componentes da PCB, você vai precisar de algumas coisinhas extras:

- Caixa impressa em 3D
- Conector Aviator
- Conector de alimentação DC (5.5 * 2.1 mm)
- Interruptor basculante (KCD1 15 * 10 mm)
- Fios e parafusos

E voilá! Está pronto para montar sua poderosa estação de solda!

---

E assim, com a tecnologia desenvolvida pela **iTS Tecnologias**, você está pronto para dominar o mundo da soldagem com estilo, precisão e aquele toque especial de inovação. Que tal começar a soldar agora mesmo?
