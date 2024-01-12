# uso-do-solo-cidade-sao-paulo
Mapa dinâmico com predominância de uso do solo no município de São Paulo e as delimitaçõe territoriais de gestão utilizadas pela SMS-SP.

Formato tmbém disponível para utilização em outros sistemas de consulta, scripts, e sites. 

Link para acessar o mapa: http://wms.geosampa.prefeitura.sp.gov.br/geoserver/geoportal/wms?service=WMS&version=1.1.0&request=GetMap&layers=MapaBase_Politico,tpcl_uso_predominancia,equipamento_saude_coordenadoria_regional,equipamento_saude_supervisao_tecnica,equipamento_saude_abrangencia_ubs,equipamento_saude_cobertura_familia,equipamento_saude_ubs_posto_centro&styles=&bbox=341000,7390000,345000,7400000&width=1850&height=850&srs=EPSG:31983&format=application/openlayers

Para alterar a extensão da "tela do mapa"Basta copiar o link acima e alterar os valores "width=1850" e "height=850"

A plataforma permite a consulta de dados em cada uma das camadas e suas tabelas de valores, para consulta via "clique". Segue abaixo a amostra de dados após um clique:

municipio
fid	cd_identificador_area_contexto	nm_area_contexto	cd_tipo_area_contexto
municipio.fid-7721ef23_18cfde8b97d_-63e8	27	SÃO PAULO	M

subprefeitura
fid	cd_identificador_subprefeitura	cd_subprefeitura	nm_subprefeitura	tx_escala	sg_fonte_original	dt_criacao	cd_tipo_discrepancia	dt_atualizacao	cd_usuario_atualizacao	sg_subprefeitura	qt_area_quilometro	qt_area_metro
subprefeitura.7	7	21	PENHA		GEOGSG	30/11/2023 00:00	100200300	30 de nov de 2023 00:00:00		PE	43.000	43358124.00

distrito_municipal
fid	cd_identificador_distrito	cd_identificador_subprefeitura	cd_distrito_municipal	nm_distrito_municipal	sg_distrito_municipal	tx_escala	sg_fonte_original	dt_criacao	dt_atualizacao	cd_usuario_atualizacao	cd_tipo_discrepancia	qt_area_quilometro	qt_area_metro
distrito_municipal.8583402	8583402	21	59	PENHA	PEN	1:5000	GEOGSG	30/11/2023 00:00	30 de nov de 2023 00:00:00		199299399	11.482	11482066.13

tpcl_uso_predominancia
fid	cd_identificador	cd_quadra_fiscal	cd_setor_fiscal	cd_quadra_setor	tx_descricao_tipo_quadra	qt_area	dt_carga_original	sg_fonte_original	cd_numero_predominancia_2015	tx_descricao_2015	cd_numero_predominancia_2014	tx_descricao_2014	cd_numero_predominancia_2013	tx_descricao_2013	cd_numero_predominancia_2012	tx_descricao_2012	cd_numero_predominancia_2011	tx_descricao_2011	cd_numero_predominancia_2010	tx_descricao_2010
tpcl_uso_predominancia.42766	42766	002	058	058002	FISCAL	20946.12	20160521	SMDU	2	Residencial horizontal medio/alto padrao	2	Residencial horizontal medio/alto padrao	2	Residencial horizontal medio/alto padrao	2	Residencial horizontal medio/alto padrao	2	Residencial horizontal medio/alto padrao	2	Residencial horizontal medio/alto padrao
tpcl_uso_predominancia.42744	42744	003	058	058003	FISCAL	18760.18	20160521	SMDU	7	Residencial e Comercio/servicos	7	Residencial e Comercio/servicos	7	Residencial e Comercio/servicos	7	Residencial e Comercio/servicos	7	Residencial e Comercio/servicos	7	Residencial e Comercio/servicos

equipamento_saude_coordenadoria_regional
fid	cd_identificador_coordenadoria_regional_saude	nm_coordenadoria_regional_saude	qt_area	dt_carga
equipamento_saude_coordenadoria_regional.5	5	SUDESTE	213.13383502600	12/05/2020 00:00

equipamento_saude_supervisao_tecnica
fid	cd_identificador_supervisao_tecnica_saude	nm_supervisao_tecnica_saude	nm_identificacao_supervisao	nm_coordenadoria_regional_saude	qt_area	dt_carga
equipamento_saude_supervisao_tecnica.16	16	PENHA	SUDESTE	COORD. REG. DE SAÚDE SUDESTE - SUPERVISÃO TÉCNICA DE SAÚDE PENHA	43.28014803860	21/07/2022 00:00

equipamento_saude_abrangencia_ubs
fid	cd_identificador	cd_numero_cadastro_nacional	nm_unidade_basica_saude	qt_area	nm_subprefeitura	dt_carga	nm_supervisao_tecnica_saude	nm_identificacao_supervisao	nm_coordenadoria_regional_saude	cd_identificador_supervisao_tecnica_saude
equipamento_saude_abrangencia_ubs.258	258	2788861	UBS VILA ESPERANÇA - CASSIO BITTENCOURT FILHO	3.56090821049	PENHA	22/07/2022 00:00	PENHA	SUDESTE	COORD. REG. DE SAÚDE SUDESTE - SUPERVISÃO TÉCNICA DE SAÚDE PENHA	16

equipamento_saude_cobertura_familia
fid	cd_identificador	cd_numero_cadastro_nacional	nm_unidade_basica_saude	qt_area	nm_subprefeitura	dt_carga	nm_supervisao_tecnica_saude	nm_identificacao_supervisao	nm_coordenadoria_regional_saude
equipamento_saude_cobertura_familia.195	195	2788861	UBS VILA ESPERANÇA - CASSIO BITTENCOURT FILHO	2.82012925693	PENHA	22/07/2022 00:00	PENHA	SUDESTE	COORD. REG. DE SAÚDE SUDESTE - SUPERVISÃO TÉCNICA DE SAÚDE PENHA

equipamento_saude_ubs_posto_centro
fid	cd_identificador	cd_identificador_tema_equipamento	nm_tema_equipamento	cd_identificador_rede_equipamento	nm_rede_equipamento	tx_rede_equipamento	cd_identificador_tipo_equipamento	nm_tipo_equipamento	tx_tipo_equipamento	cd_identificador_classe_equipamento	nm_classe_equipamento	tx_classe_equipamento	cd_identificador_esfera_administrativa_equipamento	nm_esfera_administrativa_equipamento	tx_esfera_administrativa_equipamento	cd_equipamento	nm_equipamento	tx_endereco_equipamento	nm_bairro_equipamento	cd_cep_equipamento	tx_horario_funcionamento	tx_numero_telefone	cd_equipamento_base_origem
equipamento_saude_ubs_posto_centro.120694	120694	6	SAUDE	0	SEM REDE	Sem descrição	45	Unidade Básica de Saúde	Atendimento básico em Pediatria, Ginecologia, Clínica Geral, Enfermagem e Odontologia. Principais serviços oferecidos: consultas médicas, inalações, injeções, curativos, vacinas, coleta de exames laboratoriais, tratamento odontológico, encaminhamentos par	5	UBS/POSTO DE SAÚDE/CENTRO DE SAÚDE	O PRIMEIRO CONTATO DO PACIENTE COM O SUS.	1	Municipal	Administração municipal	740	V ESPERANCA-UBS CASSIO BITTENCOURT FILHO	R MARIA CARLOTA, 631	V ESPERANCA	03647000		29576630	


Conheça também: \nGEOSampa <a href>"https://metadados.geosampa.prefeitura.sp.gov.br/geonetwork/srv/por/catalog.search#/home"</a> \nCatálogo de Metadados <a href>"https://metadados.geosampa.prefeitura.sp.gov.br/geonetwork/srv/por/catalog.search#/home"</a>


