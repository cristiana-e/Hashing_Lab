# Análise Forense de Hash de Imagens: Um Guia Estelar
Bem-vindos, investigadores da Aliança Rebelde, ao nosso laboratório de análise forense. Nosso objetivo é explorar os segredos escondidos nas imagens apreendidas das forças imperiais, utilizando técnicas de hashing. Que a força da perícia técnica esteja com vocês!


## Início da Jornada: Extração de Evidências

A saga começa com a aquisição das imagens das evidências diretamente do terminal de comando do caça TIE de Darth Vader, capturado durante uma audaciosa operação da Aliança Rebelde. Certifiquem-se de transferir as evidências para a sua estação de análise com o máximo cuidado, permitindo-nos explorar os segredos guardados sem alterar a essência do conteúdo original.


![image](https://github.com/cristiana-e/Hashing_Lab/assets/19941757/8d4c5ee0-d627-468e-ab52-7adaa1a3a7bb)



Assim que a extração estiver completa, as evidências estarão prontas para serem investigadas em sua máquina, garantindo que os dados adquiridos da imagem permaneçam intocados para futuras análises.

![image](https://github.com/cristiana-e/Hashing_Lab/assets/19941757/d29935a8-71d2-43ee-a553-be4599dc3278)



## Decifrando as evidências: Hashing

A primeira impressão ao examinar os arquivos é que estamos diante de uma curiosa situação: imagens com nomes diferentes, mas aparentemente idênticas em conteúdo. Todas elas exibem o alto oficial do Império, Darth Vader, com seus correligionários do lado sombrio.

![image](https://github.com/cristiana-e/Hashing_Lab/assets/19941757/1c4c0f10-c534-43b2-97ef-80411ad4bc31)



Ao visualizarmos a janela de propriedade das imagens, identificamos também que todas elas possuem o mesmo tamanho de arquivo (tamanho em disco está sendo ignorado neste laboratório pois não é o objetivo deste exercício).

![image](https://github.com/cristiana-e/Hashing_Lab/assets/19941757/cd5ae737-4a49-4fb2-9856-d799e3978f5d)


### Decifrando as imagens: Hashing

Um método para confirmar a identidade dos arquivos é através da análise de hash. Este processo nos permite verificar a singularidade de cada imagem, como se o código gerado fosse uma impressão digital. Cada arquivo único possuirá uma hash única.

Ao aplicar a técnica de hashing, descobrimos o seguinte resultado:
- Imagem 1 Hash MD5: 2c88e88976c4379d117854d216e36681
- Imagem 2 Hash MD5: f22d2acdbb1884af86b40d72f447eca2
- Imagem 3 Hash MD5: 2c88e88976c4379d117854d216e36681

![image](https://github.com/cristiana-e/Hashing_Lab/assets/19941757/f1728cfd-7638-4ce1-be5c-ec805a8394a2)



Este processo revela que imagens 1 e 3 são idênticas até na menor das unidades de dados, como se fossem clones imperiais, enquanto que a imagem 2 esconde segredos ainda não descobertos. Precisamos analisá-la mais a fundo para encontrarmos mais informações sobre ela.


### Aprofundando na Análise: Hexadecimais

Explorando o universo microscópico dos arquivos, utilizamos um visualizador hexadecimal para examinar os dados byte a byte.

![image](https://github.com/cristiana-e/Hashing_Lab/assets/19941757/604cfc73-cab4-4e1b-82c9-f13bd9208000)

Quando observamos byte por byte das imagens 1 e 3, é inegável que elas são idênticas. Alterando um único byte na Imagem 1 e observando as consequências, descobrimos que mesmo a menor das mudanças é detectável em nossa análise forense.


![image](https://github.com/cristiana-e/Hashing_Lab/assets/19941757/ba0607f8-ff6d-4231-a56c-536f4f4adbca)

![image](https://github.com/cristiana-e/Hashing_Lab/assets/19941757/29b7f59f-a6fb-4ad5-ac69-9415c69d48d3)


### Desvendando os Mistérios


Salvando a imagem modificada e comparando-a com as originais, percebemos que, visualmente, as imagens continuam iguais, mas sob a lente da perícia técnica, é possível revelar diferenças fundamentais.


![image](https://github.com/cristiana-e/Hashing_Lab/assets/19941757/cc2fa8cd-9641-43e4-a919-f8a7f16c1969)



Apesar das alterações, o tamanho dos arquivos se mantém.

![image](https://github.com/cristiana-e/Hashing_Lab/assets/19941757/a06f6a79-045c-4040-ac25-1212ecc0e1ba)



Mas vejam só, a modificação de um único byte alterou drasticamente a hash da imagem 1 modificada.


![image](https://github.com/cristiana-e/Hashing_Lab/assets/19941757/60983650-d78f-4d60-8375-4e1ac544efc3)



Pensanso por essa lógica, será que a imagem 2 passou por uma alteração similar?

![image](https://github.com/cristiana-e/Hashing_Lab/assets/19941757/19e73c24-b5ee-45d6-b1fc-d2e76eabde5b)



Aparentemente, os bytes são os mesmos,  mas ao analisá-la mais atentamente, descobrimos uma mensagem oculta crucial para a resistência:
- DEATH_STAR_PASSWORD IS: CutePuppies123:)

![image](https://github.com/cristiana-e/Hashing_Lab/assets/19941757/8bd69afc-a2c4-4bd1-969e-9bc7b7155ed4)


Com essa descoberta, podemos reportar à Senadora Leia Organa que a missão de inteligência foi um sucesso, desvendando a chave para um dos segredos mais bem guardados do Império (Ou nem tanto assim!).

Esta jornada através de técnicas de análise forense digital não apenas proporciona uma aventura única na análise de imagens, mas também destaca a precisão e a importância da integridade digital em investigações forenses. Que a Força esteja com você, jovem Padawan, em suas futuras incursões digitais.
