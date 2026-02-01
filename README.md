<h1 align="center">🚀 Portfólio QA: Ciclo de Validações - Sprint 4</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Concluído-brightgreen">
  <img src="https://img.shields.io/badge/Ambiente-Preview-orange">
  <img src="https://img.shields.io/badge/Testes-E2E_%26_API-blue">
</p>

<p>Este repositório documenta as validações técnicas realizadas para a plataforma <b>Lacrei Saúde</b>, focando na integridade da pipeline de dados, regras de negócio no Back-end e infraestrutura Cloud.</p>

<hr>

<h3 style="color: #2c5282;">📂 Atividade 1 - 🧪[BACK] Ajustar o endpoint de GET lacreisaude/professionals/</h3>
<p><b>Contexto:</b> Ajuste de Endpoint Profissionais. Validação de sucesso (200 OK) no mapeamento de profissão para IDs numéricos e unificação do objeto <code>clinic</code>.</p>


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

<table width="100%" style="border-collapse: separate; border-spacing: 10px; text-align: center;">
    <tr>
      <td width="50%" style="background: white; padding: 10px; border-radius: 10px; border: 1px solid #e2e8f0; box-shadow: 0 4px 6px rgba(0,0,0,0.02);">
        <img src="https://raw.githubusercontent.com/SuelemMartins/meu-portfolio-QA/main/image.TESTE.jpg" width="100%" style="border-radius: 5px;">
        <p style="margin: 10px 0 0; font-size: 0.85em; color: #2d3748;"><b>📊Validação Técnica JSON</b></p>
      </td>
      <td width="50%" style="background: white; padding: 10px; border-radius: 10px; border: 1px solid #e2e8f0; box-shadow: 0 4px 6px rgba(0,0,0,0.02);">
        <img src="https://raw.githubusercontent.com/SuelemMartins/meu-portfolio-QA/main/EVIDENCIA.IMAGEM.PNG" width="100%" style="border-radius: 5px;">
        <p style="margin: 10px 0 0; font-size: 0.85em; color: #2d3748;"><b>🔍Board Kanban no Notion</b></p>
      </td>
    </tr>
  </table>


<hr>



<h3 style="color: #c53030;">📂 Atividade 2 - 🧪 [BACK] Correção necessária no campo request_type</h3>
<p><b>Contexto:</b> Regra de Negócio. Validação do endpoint de direitos do titular com a nova funcionalidade de múltipla escolha para o campo <code>request_type</code>.</p>

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

<table width="100%" style="border-collapse: separate; border-spacing: 10px; text-align: center;">
    <tr>
      <td width="50%" style="background: white; padding: 10px; border-radius: 10px; border: 1px solid #e2e8f0; box-shadow: 0 4px 6px rgba(0,0,0,0.02);">
        <img src="https://raw.githubusercontent.com/SuelemMartins/meu-portfolio-QA/main/SPRINT04.PNG" width="100%" style="border-radius: 5px;" alt="Board Kanban Notion Sprint 04">
        <p style="margin: 10px 0 0; font-size: 0.85em; color: #2d3748;"><b>📊 Board Kanban no Notion (Sprint 04)</b></p>
      </td>
      <td width="50%" style="background: white; padding: 10px; border-radius: 10px; border: 1px solid #e2e8f0; box-shadow: 0 4px 6px rgba(0,0,0,0.02);">
        <img src="https://raw.githubusercontent.com/SuelemMartins/meu-portfolio-QA/main/IMAGEM.API.jpg" width="100%" style="border-radius: 5px;" alt="Evidência Técnica API">
        <p style="margin: 10px 0 0; font-size: 0.85em; color: #2d3748;"><b>🔍 Evidência Técnica API</b></p>
      </td>
    </tr>
  </table>

<hr>

<h3 style="color: #2b6cb0;">🚀 Atividade 3 - 🧪 [DevOps] Integração do endpoint de direitos do titular no repositório jornada-institucional</h3>
<p><b>Contexto:</b> Integração DevOps Institucional. Validação do fluxo completo confirmando a comunicação entre o front-end e a API via link de preview. Garantia de integridade com <b>retorno 201</b>.</p>

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

<table width="100%" style="border-collapse: separate; border-spacing: 10px; text-align: center;">
    <tr>
      <td width="50%" style="background: white; padding: 10px; border-radius: 10px; border: 1px solid #e2e8f0; box-shadow: 0 4px 6px rgba(0,0,0,0.02);">
        <img src="https://raw.githubusercontent.com/SuelemMartins/meu-portfolio-QA/main/IMG.SPRINT04..PNG" width="100%" style="border-radius: 5px;" alt="Sprint Board Notion">
        <p style="margin: 10px 0 0; font-size: 0.85em; color: #2d3748;"><b>📊 Board Kanban no Notion</b></p>
      </td>
      <td width="50%" style="background: white; padding: 10px; border-radius: 10px; border: 1px solid #e2e8f0; box-shadow: 0 4px 6px rgba(0,0,0,0.02);">
        <img src="https://raw.githubusercontent.com/SuelemMartins/meu-portfolio-QA/main/POST.200.PNG" width="100%" style="border-radius: 5px;" alt="Evidência Inspecionar F12">
        <p style="margin: 10px 0 0; font-size: 0.85em; color: #2d3748;"><b>🔍 Inspecionar F12 (Network 200)</b></p>
      </td>
    </tr>
  </table>
<hr>

<h3>💡 Conclusão Geral</h3>
<p>As validações confirmam que a arquitetura distribuída está em harmonia. O sistema garante a unicidade dos arquivos, a eficiência na entrega via CDN e a correta aplicação das regras de negócio no Back-end, assegurando uma experiência estável e segura para o usuário final.</p>
