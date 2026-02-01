<h1 align="center">🚀 Portfólio QA: Ciclo de Validações - Sprint 45</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Concluído-brightgreen">
  <img src="https://img.shields.io/badge/Ambiente-Preview-orange">
  <img src="https://img.shields.io/badge/Testes-E2E_%26_API-blue">
</p>

<p>Este repositório documenta as validações técnicas realizadas para a plataforma <b>Lacrei Saúde</b>, focando na integridade da pipeline de dados, regras de negócio no Back-end e infraestrutura Cloud.</p>

<hr>

<h2>🧪 Atividade 1: Ajuste de Endpoint e Mapeamento de IDs</h2>
<p><b>Foco:</b> Padronização de dados e transição estrutural da API de profissionais.</p>

<table width="100%" border="1" style="border-collapse: collapse; border: 1px solid #ddd;">
  <tr bgcolor="#f9f9f9">
    <th align="left" style="padding: 12px;">🎯 Cenários de Validação (Checklist)</th>
  </tr>
  <tr>
    <td style="padding: 12px;">
      <ul>
        <li>✅ <b>Regra de Negócio:</b> Mapeamento da propriedade <code>profession</code> para IDs numéricos (ex: ID 1 para Psicologia).</li>
        <li>✅ <b>Unificação:</b> Objeto <code>clinic</code> consolidado com indicadores de atendimento presencial e online.</li>
        <li>✅ <b>Contrato JSON:</b> Validação de campos como <code>ethnic_group</code> e <code>gender_identity</code> na resposta.</li>
        <li>✅ <b>Status Code:</b> Validação de sucesso (200 OK) no ambiente de Preview.</li>
      </ul>
    </td>
  </tr>
</table>
<br>
<h3>📸 Evidência de Execução</h3>
<p><i><b>Status:</b> Atividade Aprovada na Sprint 4 em 30/01/2026.</i></p>

<table width="100%" style="border: none; text-align: center;">
  <tr>
    <td width="50%" style="border: none;">
      <img src="https://raw.githubusercontent.com/SuelemMartins/meu-portfolio-QA/main/EVIDENCIAS3.PNG" width="100%" alt="Board de Aprovação">
      <p><small>Board de Aprovação e Checklist</small></p>
    </td>
    <td width="50%" style="border: none;">
      <img src="https://raw.githubusercontent.com/SuelemMartins/meu-portfolio-QA/main/IMAGEM.API.webp" width="100%" alt="Retorno JSON Postman">
      <p><small>Retorno JSON Postman 200 OK</small></p>
    </td>
  </tr>
</table>


<hr>

<h2>🧪 Atividade 2: Regra de Negócio e Flexibilidade</h2>
<p><b>Foco:</b> Implementação de múltipla escolha para solicitações de direitos do titular (LGPD).</p>

<table width="100%" border="1" style="border-collapse: collapse; border: 1px solid #ddd;">
  <tr bgcolor="#f9f9f9">
    <th align="left" style="padding: 12px;">🎯 Cenários de Validação (Checklist)</th>
  </tr>
  <tr>
    <td style="padding: 12px;">
      <ul>
        <li>✅ <b>Lógica de Array:</b> Validação do campo <code>request_type</code> aceitando múltiplos Enums simultâneos.</li>
        <li>✅ <b>Validação de Payload:</b> Teste de envio de requisições POST com múltiplos parâmetros de solicitação.</li>
        <li>✅ <b>Status Code:</b> Confirmação de retorno <b>201 Created</b> no ambiente de Preview.</li>
      </ul>
    </td>
  </tr>
</table>
<br>
<img src="docs/postman_atividade2.png" width="100%" alt="Evidência Postman Atividade 2">

<hr>

<h2>🧪 Atividade 3: Integração DevOps e Cloud Storage</h2>
<p><b>Foco:</b> Pipeline entre site Institucional e AWS S3/CloudFront.</p>

<table width="100%" border="1" style="border-collapse: collapse; border: 1px solid #ddd;">
  <tr bgcolor="#f9f9f9">
    <th align="left" style="padding: 12px;">🎯 Cenários de Validação (Checklist)</th>
  </tr>
  <tr>
    <td style="padding: 12px;">
      <ul>
        <li>✅ <b>Segurança:</b> Substituição do nome original do arquivo por identificador único <b>UUID</b>.</li>
        <li>✅ <b>Integração Cloud:</b> Armazenamento em diretórios S3 e entrega via link CloudFront (CDN).</li>
        <li>✅ <b>Performance:</b> Validação de tempo de resposta em requisições de upload (média 1.20s).</li>
      </ul>
    </td>
  </tr>
</table>
<br>
<img src="docs/site_institucional_sucesso.png" width="100%" alt="Evidência Site Institucional">
![Uploading image.TESTE.jpg…]()

<hr>

<h3>💡 Conclusão Geral</h3>
<p>As validações confirmam que a arquitetura distribuída está em harmonia. O sistema garante a unicidade dos arquivos, a eficiência na entrega via CDN e a correta aplicação das regras de negócio no Back-end, assegurando uma experiência estável e segura para o usuário final.</p>
