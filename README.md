<h1 align="center">🚀 Portfólio QA: Ciclo de Validações - Sprint 4 </h1>

<hr>

<h2>🧪 Atividade 1: Ajuste de Endpoint e Mapeamento de IDs</h2>

<p><b>Contexto:</b> Esta atividade consistiu na validação técnica de uma alteração estrutural no banco de dados e na API, focada na padronização de dados dos profissionais de saúde.</p>

<table width="100%" border="1" style="border-collapse: collapse; border: 1px solid #ddd; padding: 10px;">
  <tr bgcolor="#f2f2f2">
    <th align="left" style="padding: 10px;">🎯 Cenários de Validação (Checklist)</th>
  </tr>
  <tr>
    <td style="padding: 10px;">
      <ul>
        <li>✅ <b>Mapeamento de Dados:</b> Conversão da propriedade <code>profession</code> de texto para identificadores numéricos (IDs).</li>
        <li>✅ <b>Unificação de Objetos:</b> Validação do objeto <code>clinic</code> consolidado, garantindo a exibição de indicadores de atendimento presencial e online.</li>
        <li>✅ <b>Integridade de Resposta:</b> Confirmação de que o retorno da API mantém a consistência dos dados após a migração estrutural.</li>
        <li>✅ <b>Status Code:</b> Validação de sucesso (200 OK) no ambiente de Preview.</li>
      </ul>
    </td>
  </tr>
</table>

<br>

<h3>📸 Evidência de Execução</h3>
<p><i><b>Ferramenta:</b> Postman / Ambiente: Preview.</i></p>

![image TESTE](https://github.com/user-attachments/assets/d3fb115a-35a8-426e-9376-99801f1fba86)

<img width="465" height="557" alt="image" src="https://github.com/user-attachments/assets/453dff53-d3e2-493e-a365-4789926745df" />


<hr>

<h3>💡 Conclusão Técnica</h3>
<p>A validação garantiu que a transição para IDs numéricos não causou quebra de contrato na API. O objeto unificado permite uma resposta mais limpa e eficiente para o Front-end, assegurando que as informações de atendimento estejam corretas para o usuário final.</p>


<h2 align="left">🧪 Atividade 2: Regra de Negócio e Flexibilidade de Contrato (Back-end)</h2>

<p><b>Contexto:</b> Validação da implementação de múltipla escolha para o campo <code>request_type</code> no endpoint de solicitações de direitos do titular (LGPD).</p>

<table width="100%" border="1" style="border-collapse: collapse; border: 1px solid #ddd;">
  <tr bgcolor="#f9f9f9">
    <th align="left" style="padding: 12px;">🎯 Cenários de Validação (Checklist)</th>
  </tr>
  <tr>
    <td style="padding: 12px;">
      <ul>
        <li>✅ <b>Lógica de Negócio:</b> Validação da transição do campo <code>request_type</code> de valor único para suporte a múltiplos Enums.</li>
        <li>✅ <b>Validação de Payload:</b> Verificação da aceitação de arrays no JSON enviado via POST.</li>
        <li>✅ <b>Contrato de API:</b> Alinhamento com a documentação Swagger para garantir que os Enums permitidos estão operacionais.</li>
        <li>✅ <b>Status Code:</b> Confirmação de retorno <b>201 Created</b> no ambiente de Preview.</li>
      </ul>
    </td>
  </tr>
</table>

<br>

<h3>📸 Evidência de Execução</h3>
<p align="center">
 
  ![IMAGEM API](https://github.com/user-attachments/assets/248f3240-0230-4025-9601-6a811cf69007)


  <img width="479" height="497" alt="image" src="https://github.com/user-attachments/assets/173b7695-0def-466e-91e6-57da22d7db92" />



</p>

<hr>

<h3>💡 Conclusão Técnica</h3>
<p>A validação confirmou que o Back-end está processando corretamente múltiplas opções de solicitação em uma única requisição. Essa melhoria garante maior flexibilidade ao usuário e otimiza o fluxo de conformidade com a LGPD dentro da plataforma.</p>


<h2 align="left">🧪 Atividade 3: Integração DevOps e Entrega via Cloud Storage</h2>

<p><b>Contexto:</b> Validação da pipeline de dados entre o site Institucional e a infraestrutura AWS, garantindo a persistência e entrega de arquivos via CDN.</p>

<table width="100%" border="1" style="border-collapse: collapse; border: 1px solid #ddd;">
  <tr bgcolor="#f9f9f9">
    <th align="left" style="padding: 12px;">🎯 Cenários de Validação (Checklist)</th>
  </tr>
  <tr>
    <td style="padding: 12px;">
      <ul>
        <li>✅ <b>Integração de Pipeline:</b> Validação do fluxo de dados entre o repositório <code>lacrei-institucional</code> e a API de produção.</li>
        <li>✅ <b>Segurança e Padronização:</b> Verificação da regra de negócio que substitui o nome original do arquivo por um identificador único <b>UUID</b>.</li>
        <li>✅ <b>Cloud Storage (AWS):</b> Confirmação do armazenamento em diretórios S3 e entrega eficiente via link <b>CloudFront (CDN)</b>.</li>
        <li>✅ <b>UX & Rede:</b> Monitoramento via <i>Network Tab</i> para garantir tempos de resposta otimizados (média de 1.20s).</li>
      </ul>
    </td>
  </tr>
</table>

<br>

<h3>📸 Evidência de Execução</h3>
<p><i><b>Ambiente:</b> Preview / <b>Tecnologia:</b> AWS S3 & CloudFront.</i></p>
<img width="1016" height="660" alt="image" src="https://github.com/user-attachments/assets/27d1dc48-d946-4885-8f6d-feebd11fae29" />

<img width="528" height="589" alt="image" src="https://github.com/user-attachments/assets/3524d49b-8d43-472b-977d-a87328f8037d" />


<hr>

<h3>💡 Conclusão Técnica</h3>
<p>Esta validação confirma que a infraestrutura de nuvem está operando conforme os padrões de segurança e performance. O uso de UUIDs garante que não haja conflito de nomes no storage, enquanto a CDN assegura uma entrega rápida dos arquivos para o usuário final, independentemente de sua localização.</p>
