    <!DOCTYPE html>
    <!--PLEASE NAO USEM IDENTAÇÃO AUTOMATICA, ESTE CODIGO FOI IDENTADO MANUALMENTE
    COM MUITO ESFORCO, POR CAUSA DO VELOCITY O IDENTADOR AUTOMÁTICO SE PERDE, E ESTE CÓDIGO
    NAO IDENTADO FICA ILEGÍVEL -->
    <!--<meta http-equiv="access-control-allow-origin" content="http://www.example.org">-->
    <!--<meta http-equiv="access-control-allow-origin" content="https://localhost:8181/conecte">-->
    <meta http-equiv="access-control-allow-origin" content="https://localhost:8181/conecte/pep/site/main/default.jsf">
    <!--<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />-->
    <html xmlns="http://www.w3.org/1999/xhtml">
        <head>
            <title>Wareline - Tecnologia em saúde</title>  
            <link href="https://localhost:8181/editor/css/font-awesome.min.css" type="text/css" rel="stylesheet"/>
            <meta name="viewport" content="width=device-width, initial-scale=1.0" />
            <link href="https://localhost:8181/editor/css/jquery-ui.min.css" rel="stylesheet" media="screen" />
            <link href="https://localhost:8181/editor/css/bootstrap.min3.3.7.css" rel="stylesheet" media="screen" />
            <link href="https://localhost:8181/editor/css/novoLayout/alteracoesCamposDigitaveisFormulario.css" rel="stylesheet" media="screen" />
            <link href="https://localhost:8181/editor/css/pages/mesclagem/formularioMesclagem.css" rel="stylesheet" media="screen" />
            <link href="https://localhost:8181/editor/css/main-styles.css" rel="stylesheet" media="screen">
            <link href="https://localhost:8181/editor/css/demo_table.css" rel="stylesheet" media="screen">

            <!--[if lt IE 9]> 
                <script src="js/html5shiv.js"></script>
                <script src="js/respond.min.js"></script>
            <![endif]-->
            <!--MESMO QUE UTILIZADO NO PRIMEFACES 5.3-->
            <script type="text/javascript" src="https://localhost:8181/editor/js/jquery_v1.12.0.js"></script>

            <script type="text/javascript" src="https://localhost:8181/editor/js/fontawesome.js"></script> 
            <script type="text/javascript" src="https://localhost:8181/editor/js/doT.js"></script>
            <script type="text/javascript" src="https://localhost:8181/editor/js/jquery.loading.js"></script>
            <script type="text/javascript" src="https://localhost:8181/editor/js/pages/mesclagem/mesclagemControl.js"></script>

            <script type="text/javascript" src="https://localhost:8181/editor/js/jquery.dataTables.min_1.10.15.js"></script> 
            <script type="text/javascript" src="https://localhost:8181/editor/js/dataTables.Plugins.js"></script>

            <script type="text/javascript" src="https://localhost:8181/editor/js/dataTables.bootstrap.min.js"></script>
            <script type="text/javascript" src="https://localhost:8181/editor/js/dataTables.jqueryui.min.js"></script>

            <script type="text/javascript" src="https://localhost:8181/editor/js/jquery.mask1.14.10.js"></script>
            <script type="text/javascript" src="https://localhost:8181/editor/js/ckeditor.js"></script>
            <script type="text/javascript" src="https://localhost:8181/editor/js/jquery-ui.min.js"></script>
            <script type="text/javascript" src="https://localhost:8181/editor/js/jquery.mb.browser.min.js"></script>
            <script type="text/javascript" src="https://localhost:8181/editor/js/jquery.webkitresize.js"></script>
            <script type="text/javascript" src="https://localhost:8181/editor/js/bootstrap.min.js"></script>
            <script type="text/javascript" src="https://localhost:8181/editor/js/strings.js"></script>
            <script type="text/javascript" src="https://localhost:8181/editor/js/strings.js"></script>
            <!--<script type="text/javascript" src="https://localhost:8181/editor/js/utils.js"></script>--> 
            <script type="text/javascript" src="https://localhost:8181/editor/js/pages/mesclagem/alteracoesJSMesclagem.js"></script> 
            <!--<script src="https://igorescobar.github.io/jQuery-Mask-Plugin/js/jquery.mask.min.js"></script>--> 
            <script type="text/javascript" src="https://localhost:8181/editor/js/jquery.mask.min.js"></script>


            <!--TIMEPICKER-->
            <link href="https://localhost:8181/editor/css/jquery.ui.timepicker.css" type="text/css" rel="stylesheet"/>
            <script type="text/javascript" src="https://localhost:8181/editor/js/jquery.ui.timepicker.js"></script> 
            <script type="text/javascript" src="https://localhost:8181/editor/js/jquery.ui.core.min.js"></script> 
            <script type="text/javascript" src="https://localhost:8181/editor/js/mascaras-campo-digitado.js"></script> 

            <style>
                .ui-timepicker-hour-cell a, .ui-timepicker-minute-cell a{padding-left: 15px!important;padding-right: 15px!important}
                .ui-timepicker-table td a{display: initial;}
                .periods{display: none}
                .cke_ltr{width: 155px;}
                @media screen and (min-width: 992px) {
                    fieldset {
                        width: 100% !important;
                    }
                    .col-md-6 {
                        width:100%;
                    }
                }

                .afina_linha {
                    padding: 5px !important;
                } 
                
                .col-prod-selec, .col-cid-selec, .col-diag-selec, .col-tabppadr-selec, .col-cadmedic-selec, 
                .col-txtfrase-selec, .col-tabintsv-selec {
                    width: 10% !important;
                }
                .col-prod-codigo, .col-cid-codigo, .col-diag-codigo, .col-cadmedic-codigo, 
                .col-txtfrase-codigo, .col-tabintsv-codigo, .col-laudos-selec, .col-laudos-numtexto  {
                    width: 10% !important; 
                }
                .col-txtfrase-numcampo {
                    width: 0% !important; 
                }
                .col-txtfrase-codigo, .col-txtfrase-desc  {
                    width: 30% !important; 
                }
                .col-tabppadr-codigo-tabela, .col-tabppadr-codigo-servico  {
                    width: 15% !important; 
                }
                .col-prod-desc, .col-cid-desc, .col-diag-desc, .col-cadmedic-desc, 
                .col-tabintsv-desc {
                    width: 80% !important; 
                }
                .col-tabppadr-desc, .col-laudos-desc {
                    width: 60% !important; 
                }
                .col-laudos-visual {
                    width: 20% !important; 
                }

                #form-entrada {
                    width: 100% !important;
                }

            </style>

            <!--FIM TIMEPICKER-->
        </head>
        <body class="camposDigitaveis" onload="javascript:carregaLocalStorage()">
            <div id="wrap">
                <div id="dialog"></div>

                <!--LOADING-->
                <div class="carregando_div">   
                    <div id="carregando">
                        <img style="height:32px;" src="img/loading.gif" alt="Aguarde"><span>   Carregando...</span>
                    </div>
                </div>
                <!--FIM LOADING-->
                <div id="cadastro01" class="panel panel-default container">
                    <div class="panel-heading">
                        <h3>QA TESTE</h3>
                    </div>
                    <div class="panel-body">
                        <div class="col-md-12">
                            <div id="content">
                                                        <div class="informarCamposDigitaveis">
                                <div class="mensagens-erro" style="display: none">
                                    <button type="button" onclick="fecharMensagens()" class="fecharErros">X</button>
                                    <ul/>
                                </div>

                                <form class="form-horizontal col-md-12" id="form-entrada">
                                    <input type="hidden" id="953" />
                                                                                                                
                                                                                <input type="hidden" id="numtextoRequest" value="53" />
                                        <input type="hidden" id="cabecalhoRequest" value="" />
                                        <input type="hidden" id="rodapeRequest" value="" />
                                        <input type="hidden" id="atendimentosParaRepetirRequest" value="" />
                                                                                    <div class="form-group">
                                                                                                                                                                    <div class="col-md-2">
                                                <label for="D002" style="font-size: 13px;font-weight: bold; word-wrap: anywhere;">
                                                     aew 
                                                </label>
                                            </div>
                                                                                   console.log(LAUDO);
                                                                                                                            </div>	
                                                                                                                                                    <hr>
                                    <div class="form-group"> 
                                        <input type="hidden" id="isImpressao" value="N" />
                                        <input id="botaoMesclar" 
                                            type="button" 
                                            class="btn btn-primary btMescla pull-right margin-right-30" 
                                            value="Salvar/Imprimir" 
                                            data-contemErros="false" 
                                            onclick="mesclar()"/>
                                    </div> 
                                    <div class="modal fade" 
                                        id="modalCamposDigitados">
                                        <div class="modal-dialog">
                                            <div class="modal-content">
                                                <div class="modal-header">
                                                    <h4 class="modal-title">Alertas Relatório</h4>
                                                </div>
                                                <div class="modal-body" 
                                                    id="corpoModalLaudos" 
                                                    style="max-height: 300px;overflow: auto;">
                                                    <p id="info"></p>
                                                </div>
                                                <div class="modal-footer">
                                                    <button type="button" 
                                                        class="bt btn btn-primary" 
                                                        data-dismiss="modal">
                                                        OK
                                                    </button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div id="modalLaudos$campo.acronimo$campo.pk.numTexto" 
                                        class="modal fade in">
                                        <div class="modal-dialog modal-lg">
                                            <div class="modal-content">
                                                <div class="modal-header">
                                                    <button class="close" 
                                                        style="margin-top: -17px!important;" 
                                                        onclick="fecharModalLaudos('#' + modalLaudos$campo.acronimo$campo.pk.numTexto);" 
                                                        data-dismiss="modal" 
                                                        type="button">
                                                        <span aria-hidden="true" 
                                                            style="font-size: 30px;">
                                                            ×
                                                        </span>
                                                        <span class="sr-only">
                                                            Close
                                                        </span>
                                                    </button>
                                                    <h4 class="modal-title">
                                                        Consulta de Laudo Padrao
                                                    </h4>
                                                </div>
                                                <div class="modal-body" 
                                                    id="corpoModalLaudos">
                                                    <table id="tableModalLaudos$campo.acronimo$campo.pk.numTexto" 
                                                        style="width: 100%;font-size: 10px" 
                                                        class="tbl-dados table table-striped table-bordered table-hover">
                                                    </table> 
                                                </div>
                                                <div class="modal-footer" 
                                                    id="btsModalLaudos">
                                                    <button type="button" 
                                                        id="cancel2$campo.acronimo$campo.pk.numTexto" 
                                                        class="btn btn-default pull-left" 
                                                        data-dismiss="modal" 
                                                        onclick="fecharModalLaudos('#' + modalLaudos$campo.acronimo$campo.pk.numTexto);">
                                                            Fechar
                                                    </button>
                                                    <button type="button" 
                                                        class="btn btn-default" 
                                                        onclick="substituirLaudosNoTexto(this.id)" 
                                                        id="incluiLaudos$campo.acronimo$campo.pk.numTexto">
                                                        Substituir
                                                    </button>
                                                    <button type="button" 
                                                        class="btn btn-success" 
                                                        onclick="incluiLaudosNoTexto(this.id, $campo.maxLength)" 
                                                        id="incluiLaudos$campo.acronimo$campo.pk.numTexto">
                                                        Inserir
                                                    </button>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                                             
                                </form>
                            </div>
                                                        </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class='slower-ajax' style='display:none; position: fixed;left: 0;right: 0;top: 0;bottom: 0;z-index: 5000; flex: 1 0 auto;justify-content: center;align-items: center;flex-direction: column;'>
                <div style='background-color: #fff; opacity: .8; border-radius: 6px; padding: 100px; display: flex;flex: 0;justify-content: center;align-items: center;flex-direction: column;box-shadow: 0px 0px 5px 0px rgba(0,0,0,.2);'>
                    <img src="https://localhost:8181/editor/img/progress2.gif" alt="Carregando..." />
                    <img src="https://localhost:8181/editor/img/wareline-logo.png" alt="Carregando..." />
                </div>
            </div>
        </body>
    </html>

<script type="text/javascript">
    document.addEventListener('DOMContentLoaded', 
        function() {
            ajustaApresentacaoCampoTextoTabulado();
            ajustaApresentacaoListaFixaTabulada();
            topoTela();
        }, false
    );

    function ajustaApresentacaoCampoTextoTabulado() {
        const demoClasses = document.querySelectorAll('.ajustaApresentacaoCampoTextoTabulado');
        demoClasses.forEach(element => {
              var i = element.getAttribute("maxlength");
              let conteudo = "display: inline-block; margin-right: 10px !important; margin-bottom: 5px !important; width: " + (i*30 > 899 ? 860 : i*30) + "px";
              element.setAttribute("style",conteudo);
        });
    }

    function ajustaApresentacaoListaFixaTabulada() {
        const tabClasses = document.querySelectorAll('.ajustaApresentacaoListaFixaTabulada');
        tabClasses.forEach(element => {
              element.setAttribute("style","width: 250px; display: inline-block;");  
              var elementoPai = element.parentElement;
              let conteudo = "display: inline-block; margin-right: 10px !important; margin-bottom: 5px !important; width: 300px";
              elementoPai.setAttribute("style",conteudo);
        });
    }

    var camposDigitaveis = {"D002":{"origemInfo":"DIGITADO","sequenciaCampo":2,"acronimo":"D002","nome":"aew","mascara":"","maxLength":9999,"maxlinhas":1,"codigoBarras":false,"rotulo":"aew","obrigatorio":false,"invisivel":false,"tirabranco":false,"tabulacao":false,"controle":"LAUDO","valorPadrao":"","valorResultvl":"","qtdOpcoes":0,"numerico":false,"numero":"53","limitcond":"N","valnorchec":"N","laudo":true,"opcoes":[]}};
    var laudosInclusao = [];
    var produtosInclusao = [];
    var cidInclusao = [];
    var diagInclusao = [];
    var tabppadrInclusao = [];
    var cadmedicInclusao = [];
    var tabintsvInclusao = [];
    var txtfraseInclusao = [];
    var listaCorpoLaudos = [];
    var listaCorpoProdutos = [];
    var listaCorpoCid = [];
    var listaCorpoDiag = [];
    var listaCorpoTabppadr = [];
    var listaCorpoCadmedic = [];
    var listaCorpoTabintsv = [];
    var listaCorpoTxtfrase = [];
    var corpo, cabecalho, rodape, edc;
    init();
    geraCkeditor();
    function geraCkeditor() {
        $('textarea:not(.campoDeArea)').each(function (index) {
            if (!$(this).hasClass("campoDeArea")) {
            var tamanho = $(this).attr("id").indexOf("laudo") !== -1 ? 700 : 250;
            var valorStringDoTamanho = $(this).attr("data-maxlen");
            var valorInteiroDoTamanho = parseInt(valorStringDoTamanho); 
            if (valorInteiroDoTamanho <= 100) {
                tamanho = 80;
            }
            if (valorInteiroDoTamanho > 100 && valorInteiroDoTamanho < 400) {
                tamanho = 350;
            }
            CKEDITOR.replace($(this).attr("id"), {
                toolbar: ('Basic2'),
                height: tamanho,
                startupFocus: false,
                wordcount: {
                    showCharCount: true,
	            maxCharCount: valorStringDoTamanho }
            });

            }
        });

        var form = jQuery("#form-entrada");
        form.find('input:text, input:checkbox, select, textArea').each(function (i, elem) {
            if (elem.nodeName === 'TEXTAREA') {
                if (!$(elem).hasClass("campoDeArea") && $(this).attr('data-id') !== undefined) {
                    CKEDITOR.instances[$(this).attr('data-id')].on('change', function () {
                        var valor = eval('CKEDITOR.instances[$(this).attr("name")].getData()');
                        window.localStorage.setItem('CD_VIVO_' + $(this).attr("name"), valor);
                    });
                }
            }
        });

    }
    function init(camposDigitaveis) {
        $('#botaoMesclar').removeAttr('disabled');
        $('#botaoMesclar').removeClass('botaoDisabled');
        camposDigitaveis = {"D002":{"origemInfo":"DIGITADO","sequenciaCampo":2,"acronimo":"D002","nome":"aew","mascara":"","maxLength":9999,"maxlinhas":1,"codigoBarras":false,"rotulo":"aew","obrigatorio":false,"invisivel":false,"tirabranco":false,"tabulacao":false,"controle":"LAUDO","valorPadrao":"","valorResultvl":"","qtdOpcoes":0,"numerico":false,"numero":"53","limitcond":"N","valnorchec":"N","laudo":true,"opcoes":[]}};
        campoSubstituivel = false;
        campoRepetir = false;
        //campoAtendimentosParaRepetir = ;
        jQuery('body .informarCamposDigitaveis .mensagens-erro').hide();
        initCombo();
        carregarCalendarios();
        configurarMascaras();
        alteracoesAdicionaisMesclagem();
    }
    function initCombo() {
        var combos = jQuery('body .informarCamposDigitaveis .combo');
        combos.each(function (i, elem) {
            var combo = $(elem);
            var input = combo.find('input');
            var lista = combo.find('ul');
            combo.find('button').click(function () {
                if (lista.hasClass('close')) {
                    lista.removeClass('close');
                } else {
                    lista.addClass('close');
                }
            });
            lista.find('li').each(function (j, e) {
                var li = $(e);
                li.click(
                    function () {
                        input.val(li.attr('data-value'));
                        lista.addClass('close');
                });
            });
        });
    }

    function carregarCalendarios() {
        jQuery(function ($) {
            $.datepicker.regional['pt-BR'] = {closeText: 'Fechar', 
                prevText: '&#x3c;Anterior', 
                nextText: 'Pr&oacute;ximo&#x3e;', 
                currentText: 'Hoje', 
                monthNames: ['Janeiro', 'Fevereiro', 'Mar&ccedil;o', 'Abril', 'Maio', 'Junho', 'Julho', 'Agosto', 'Setembro', 'Outubro', 'Novembro', 'Dezembro'], 
                monthNamesShort: ['Jan', 'Fev', 'Mar', 'Abr', 'Mai', 'Jun', 'Jul', 'Ago', 'Set', 'Out', 'Nov', 'Dez'], 
                dayNames: ['Domingo', 'Segunda-feira', 'Ter&ccedil;a-feira', 'Quarta-feira', 'Quinta-feira', 'Sexta-feira', 'Sabado'], 
                dayNamesShort: ['Dom', 'Seg', 'Ter', 'Qua', 'Qui', 'Sex', 'Sab'], 
                dayNamesMin: ['Dom', 'Seg', 'Ter', 'Qua', 'Qui', 'Sex', 'Sab'], 
                weekHeader: 'Sm', 
                dateFormat: 'dd/mm/yy', 
                firstDay: 0, 
                isRTL: false, 
                showMonthAfterYear: false, 
                yearSuffix: ''};
            $.datepicker.setDefaults($.datepicker.regional['pt-BR']);
        });
        //Calendarios
        var calendarios = jQuery('body .informarCamposDigitaveis div.calendar');
        calendarios.each(function (i, e) {
            var calendario = $(e);
            var input = calendario.find('input[type="text"]');
            var mk = input.attr('data-mascara').toUpperCase();
            var mascara = mk === 'DD/MM/YY HH:MM' ? 'dd/mm/yy'
                : mk === 'DD/MM/Y HH:MM' ? 'dd/mm/y'
                : mk === 'DD/MM/YY' ? 'dd/mm/yy'
                : mk === 'DD/MM/Y' ? 'dd/mm/y' : '00:00';
            var datepickerConfig = {
                dateFormat: mascara,
                changeMonth: true,
                changeYear: true,
                showButtonPanel: true
            };
            var datepickerBundle = jQuery.datepicker.regional[ 'pt-PT' ];
            input.datepicker(datepickerConfig, datepickerBundle);
            calendario.find('button').click(function () {
                input.datepicker('show');
            });
        });
        //Campos Horas
        var cHora = jQuery('.camposDigitaveis .hora');
        cHora.each(function (i, e) {
            var hora = $(e);
            var input = hora.find('input[type="text"]');
            $(e).find('input[type="text"]').timepicker({
                showAnim: 'blind',
                showOn: 'focus',
                hourText: 'Hora',
                minuteText: 'Minuto',
                rows: 6,
                showCloseButton: true,
                closeButtonText: 'OK',
                showNowButton: true,
                nowButtonText: 'Agora',
                showDeselectButton: true,
                deselectButtonText: 'Cancelar'
            });
            hora.find('button').click(function () {
                input.timepicker('show');
            });
        });
    }

    function configurarMascaras() {
        jQuery('.camposDigitaveis .masked').each(function (i, elem) {
            elem = jQuery(elem);
            var mk = elem.attr('data-mascara').toUpperCase();
            if (mk === 'DD/MM/YY HH:MM' || 
                mk === 'DD/MM/Y HH:MM' ||
                mk === 'DD/MM/YY' ||
                mk === 'DD/MM/Y' ||
                mk === 'HH:MM') {
                var mascara = mk === 'DD/MM/YY HH:MM' ? '00/00/0000'
                    : mk === 'DD/MM/Y HH:MM' ? '00/00/00'
                    : mk === 'DD/MM/YY' ? '00/00/0000'
                    : mk === 'DD/MM/Y' ? '00/00/00' : '00:00';
                //Estilo 01 - dd/mm/yy HH:mm    '00/00/0000 00:00'
                //Estilo 02 - dd/mm/y HH:mm     '00/00/00 00:00'
                //Estilo 03 - dd/mm/yy          '00/00/0000' 
                //Estilo 04 - dd/mm/y           '00/00/00' 
                //Estilo 05 - HH:mm             '00:00'
                $(elem).mask(mascara);
            }
        });
    };


    function mesclar() {
        if (isTamanhoDeCamposDigitadosInconsistentes()) {
            return;
        }
        var erro = null;
//        if (!validarCampos()) {
//            return;
//        }
        var campos = getValoresCamposDigitados();
        var sair = false;
        var params = {};
        $(params).push({"numeroTexto":53,"valorPk1":"24","operadorLogado":"000001"});
        params.qtdCamposDigitados = campos.length;
        params.camposDigitados = campos;
        params.finalizarMesclagem = true;
        params.mesclagemComCamposDigitados = true;
        params.requisicao = $('body').hasClass('naoVisulAosalvar') ? '7' : '2';
        params.numTexto = $('#numtextoRequest').val();
        params.numeroTexto = $('#numtextoRequest').val();
        params.numeroCabecalho = $('#cabecalhoRequest').val();
        params.numeroRodape = $('#rodapeRequest').val();
        params.valorPk1 = retornaValorUrlGet('valorPk1');
        params.valorPk2 = retornaValorUrlGet('valorPk2');
        params.valorPk3 = retornaValorUrlGet('valorPk3');
        params.valorPk4 = retornaValorUrlGet('valorPk4');
        params.operadorLogado = retornaValorUrlGet('operadorLogado');
        params.impredir = retornaValorUrlGet('impredir');
        params.edc = $('#edc').val();
        params.sistemaEditor = window.location.pathname;
        params.origemInfo = 'D';
        params.substituicao = false;
        params.repetir = false;
        params.atendimentosParaRepetir = $('#atendimentosParaRepetirRequest').val(); //;
        params.isImpressao = $('#isImpressao').val();
//      alert(JSON.stringify(params)); 
        jQuery('.slower-ajax').css('display','flex');
        jQuery.ajax({
            type: 'POST',
            url: '/editor/mesclagem', /*/editor/mesclagem*/
            data: params,
            datatype: 'json',
            async: false
        }).done(function (ret) {
            if (ret === 'FecharImpressao') {
                sair = true;
                limpaCDVivos();
            } else {
                //$("#carregando").css('display', 'none');
                var texto = ret.split("&&ValorEdc&&")[0];
                edc = ret.split("&&ValorEdc&&")[1];
                cabecalho = texto.split("&&TEXTO&&")[0];
                corpo = texto.split("&&TEXTO&&")[1];
                rodape = texto.split("&&TEXTO&&")[2];
                numtexto = texto.split("&&TEXTO&&")[3];
            }
            
            // $('body').html($('<div>').addClass('w-resultado-mesclagem').html(ret));
        }).fail(function (jqXHR, textStatus, errorThrown) {
            jQuery('.slower-ajax').css('display','none');
            //alert('testeeee Fail: ' + textStatus)
            erro = true;
            //$("#carregando").css('display', 'none');
            alert(jqXHR.responseText || 'Ocorreu um erro durante a mesclagem. Se esse problema persistir contate o suporte.');
            sair = true;
        });
        if (sair) {
            parent.sair();
            jQuery('.slower-ajax').css('display','none');
        } else {
            //abrirPdf(cabecalho + corpo + rodape, edc, numtexto);
            //alert("numtexto = " + numtexto + ",corpo = " +  corpo + ",rodape = " + rodape + ", edc = " + edc + ",cabecalho = " + cabecalho);
            if (numtexto === undefined && corpo === undefined && rodape === undefined && edc === undefined && cabecalho !== undefined) {
                jQuery('.camposDigitaveis').html(cabecalho);
            } else {
                abrirPdf(cabecalho,corpo,rodape, edc, numtexto);
                limpaCDVivos();
            }
        }
    }

    function abrirPdf(cabecalho, html, rodape, edc, numtexto) {
        var url = '' + window.location.href.split("?")[0];
        var htmlFinal = acertaSimbolos(html);
        var htmlCabecalho = acertaSimbolos(cabecalho);
        var htmlRodape = acertaSimbolos(rodape);
        var form = $('<form action="' + url + '" method="post">' +
            '<input type="text" name="edc" value="' + edc + '" style="display: none;"/>' +
            '<input type="text" name="numtexto" value="' + numtexto + '" style="display: none;"/>' +
            '<textArea name="numCabecalho" style="display: none;" >' + htmlCabecalho + '</textArea>' +
            '<textArea name="numRodape" style="display: none;" >' + htmlRodape + '</textArea>' +
            '<input type="text" name="requisicao" value="16" style="display: none;"/>' +
            '<textArea  name="html" style="display: none;" >' + htmlFinal + '</textArea></form>');
        $('body').append(form);
        form.submit();
    }

    function isTamanhoDeCamposDigitadosInconsistentes() {
        var isTamanhoDeCamposDigitadosInconsistentes = false;
        var erros = [];
        var i = 0;
        var form = jQuery("#form-entrada");
        form.find('input:text, input:checkbox, select, textArea').each(function (i, elem) {
            if (elem.nodeName === 'TEXTAREA') {
                if (!$(elem).hasClass("campoDeArea")) {
                valor = eval('CKEDITOR.instances[$(elem).attr("id")].getData()');
                var componente = jQuery(elem);
                var maxlengh = (componente.attr("data-maxlen"));
                var caracteresTextArea = contaCaracCKEDITOR(valor);
                if (caracteresTextArea > maxlengh) {
                    isTamanhoDeCamposDigitadosInconsistentes = true;
                    erros[i] = "O campo: " + $(this).attr("data-rotulo") + " Ultrapassa o limite de Caracteres estipulado no seu cadastro. Foram digitados: " + caracteresTextArea + " caracteres, limite estabelecido: " + maxlengh + ".";
                    i++;
                }
                }
            }
        });
        if (isTamanhoDeCamposDigitadosInconsistentes) {
            imprimeErros(erros);
        } else {
            isTamanhoDeCamposDigitadosInconsistentes = !validarCampos();
            //alert("isTamanhoDeCamposDigitadosInconsistentes = " + isTamanhoDeCamposDigitadosInconsistentes);
        }
        return isTamanhoDeCamposDigitadosInconsistentes;
    } 

    function imprimeErros(erros) {
        var ul = jQuery('.informarCamposDigitaveis .mensagens-erro ul');
        ul.html("");
        for (i = 0; i < erros.length; i++) {
            var li = ul.append('<li>' + erros[i] + '</li>');
        }
        topoTela();
        jQuery('body .informarCamposDigitaveis .mensagens-erro').show();
    } 


    function getValoresCamposDigitados() {
        var ret = [];
        var eML = "";
        var form = jQuery('body div.informarCamposDigitaveis form');
        var dataFilds = [];
        form.find('input:text, input:checkbox, select, textArea').each(function (i, elem) {
            eML = "";
            var noPut = false;
            var componente = jQuery(elem);
            var acronimo = componente.attr('data-acronimo');
            var valor = componente.val();
            var numeroTexto = componente.attr('data-numtexto');
            var tipo = componente.attr('data-tipo');
            var tipoControle = componente.attr('data-tipoControle');
            var tipoCampo = componente.attr('data-tipoCampo');
            if (componente.attr('type') === 'checkbox') {
                valor = componente.is(':checked') ? 'S' : 'N';
            } else if ((componente.attr('type') === 'text') && (componente.hasClass('masked')) && !(componente.hasClass('hasTimepicker'))) {
                valor = componente.val();
            } else if ((componente.attr('type') === 'text') && (componente.hasClass('hasTimepicker'))) {
                noPut = true;
                var temOCampo = false;
                for (var i = 0; i < ret.length; i++) {
                    console.log(ret[i].campo);
                    if ("undefined"!==typeof ret[i].campo && ret[i].campo.acronimo === acronimo) {
                        temOCampo = true;
                        ret[i].valor = ret[i].valor + " " + componente.val();
                    }
                }
                if (!temOCampo) {
                    noPut = false;
                }
            }
            if (elem.nodeName === 'TEXTAREA') {
                if (!$(elem).hasClass("campoDeArea")) {
                    valor = eval('CKEDITOR.instances[$(elem).attr("id")].getData()');
                    var maxlengh = (componente.attr("data-maxlen"));
                    var caracteresTextArea = contaCaracCKEDITOR(valor);
                    if (caracteresTextArea > maxlengh) {
                        eML = "O campo: " + $(this).attr("data-rotulo") + " Ultrapassa o limite de Caracteres estipulado no seu cadastro. Foram digitados: " + caracteresTextArea + " caracteres, limite estabelecido: " + maxlengh + ".";
                    }
                }
            }
            if (!noPut) {
                ret.push({campo: camposDigitaveis[acronimo], valor: valor, tipoCampo: tipoCampo, tipoControle: tipoControle, erroML: eML, numeroTexto: numeroTexto});
            }
        });
        form.find('div.radioGroup ul').each(function (i, elem) {
            var componente = jQuery(elem);
            var selecionado = componente.find("li input[type='radio']:checked");
            var acronimo = selecionado.attr("data-acronimo");
            var valor = selecionado.val();
            var numeroTexto = selecionado.attr('data-numtexto');
            var tipoCampo = selecionado.attr('data-tipoCampo');
            var tipoControle = selecionado.attr('data-tipoControle');
            if (componente.size() <= 0) {
                valor = "";
            }
            ret.push({campo: camposDigitaveis[acronimo], valor: valor, tipoCampo: tipoCampo, tipoControle: tipoControle, numeroTexto: numeroTexto});
        });
        return ret;
    }
    function contaCaracCKEDITOR(textoRecebido) {
        var texto = textoRecebido;
        texto = texto.replace(/(<([^>]+)>)/ig, "");
        var valores = "&nbsp;-\n-\t";
        for (var i = 0; i < valores.split("-").length; i++) {
            valor = valores.split("-")[i];
            do {
                texto = texto.replace(valor, "");
            } while (texto.indexOf(valor) !== -1);
        }
        return texto.length;
    }
    function acertaSimbolos(text) {
        if (typeof text === "undefined") {
            return "";
        }
        text = text.toString();
        do {
            text = text.replace('"', "&&TROCAASPAS&&");
        } while (text.indexOf('"') !== -1);
        do {
           text = text.replace('&nbsp;', "&&TROCAESPACO&&");
        } while (text.indexOf('&nbsp;') !== -1);
        return text;
    }
    function validarCampos() {
        var alertNatela = '';
        var erros = [];
        var cont = 0;
        var resposta;
        $('.camposDigitaveis .required').each(function (i, elem) {
            var componente = jQuery(elem);
            //var labelCampo = componente.parent().children().first().html().replace('\*', '').trim() || componente.parent().parent().children().first().html().replace('\*', '').trim();
            var labelCampo = componente.attr('data-rotulo');
            var acronimo = componente.attr('data-acronimo');
            var campoInvalido = false;
            if (componente.hasClass('radioGroup')) {
                //campoInvalido = componente.find('input[type="radio"]:checked').length < 1;
                //alert(campoInvalido + "," + (!campoInvalido) + ", teste 1");
                campoInvalido = true;
            } else if (componente.hasClass('combo')) {
                campoInvalido = componente.find('input[type="text"]').val();
                console.log(componente);
                console.log(campoInvalido);
            } else if (jQuery(elem).hasClass('ckEditorText')) {
                //campoInvalido = CKEDITOR.instances[jQuery(elem).attr('id')].getData() === '';
                var valor = eval('CKEDITOR.instances[$(elem).attr("id")].getData()');
                campoInvalido = valor.trim() !== '';
                console.log(elem);
                console.log(jQuery(elem).attr('id'));
                console.log(campoInvalido);
            } else {
                campoInvalido = componente.val();
                console.log("labelCampo = " + labelCampo + ", componente.attr('data-rotulo') = " + componente.attr('data-rotulo'));
                console.log(componente);
                console.log(campoInvalido);
            }
            if (!campoInvalido) {
                erros.push('Campo obrigatório "{0}" não preenchido.'.format(labelCampo));
            }
        });
        $('.campoCPF').each(function (i, elem) {
             console.log('entrou em rotina de cpf...');
            var cpfValido = false;
            var componente = jQuery(elem);
            var cpf = componente.val();
            console.log(cpf);
            cpfValido = validaCPF(cpf);
            if (!cpfValido) {
                erros.push('O Cpf [' + cpf + "] é inválido.");
            }
        });
        var campos = getValoresCamposDigitados();
        for (var j = 0; j < campos.length; j++) {
            if (campos[j].erroML != null && campos[j].erroML != "") {
             //alert('AQUIIIIIIIIIIIII' + JSON.stringify(campos[j]));
               erros.push(campos[j].erroML);
            }
        }
      //alert(JSON.stringify(erros)); 
        var params = {"numeroTexto":53,"valorPk1":"24","operadorLogado":"000001"};
        params.qtdCamposDigitados = campos.length;
        params.camposDigitados = campos;
        params.action = 'consistenciaErroDigLimite';
        params.edc = $('#edc').val(); // "2267T"; 
        console.log(params);
        jQuery.ajax({
            type: 'POST',
            url: '/editor/TextoControl',
            data: params,
            async: false,
        }).done(function (ret) {
            console.log(ret);
            if (ret != '') {
                var consistencia = ret.respostas[0].consistencia, 
                    erroDig = ret.respostas[0].erroDig, 
                    limite = ret.respostas[0].limite, 
                    respostaFinalAlert = "";
                /* *********TESTES CONSISTENCIAS********* */
                if (!isEmpty(consistencia)) {
                    if (consistencia.indexOf("#") != -1) {
                        for (var i = 0; i < consistencia.split("#").length; i++) {
                            if (consistencia.split("#")[i] != 'null') {
                                if (consistencia.split("#")[i].split("!@")[0] == 'M') {
                                    respostaFinalAlert = respostaFinalAlert == "" ? "&bull; " + consistencia.split("#")[i].split("!@")[1] + "</br>&nbsp;&nbsp;&nbsp;&nbsp;&#8627;Descricao: " + consistencia.split("#")[i].split("!@")[2] + "<br>" : respostaFinalAlert + "\n&bull; " + consistencia.split("#")[i].split("!@")[1] + "</br>&nbsp;&nbsp;&nbsp;&nbsp;&#8627;Descricao: " + consistencia.split("#")[i].split("!@")[2] + "<br>";
                                } else if (consistencia.split("#")[i].split("!@")[0] == 'B') {
                                    erros.push(consistencia.split("#")[i].split("!@")[1] + "<br>&nbsp;&nbsp;&nbsp;&nbsp;&#8627;Descri&ccedil;&atilde;o: " + consistencia.split("#")[i].split("!@")[2] + "<br>");
                                }
                            }
                        }
                    } else {
                        if (consistencia.split("#")[i] != 'null') {
                            if (consistencia.split("!@")[0] == 'M') {
                                respostaFinalAlert = "‣ " + consistencia.split("!@")[1] + "\nDescricao: " + consistencia.split("!@")[2] + "<br>";
                            } else if (consistencia.split("!@")[0] == 'B') {
                                erros.push(consistencia.split("!@")[1] + "<br>&#8227; Descri&ccedil;&atilde;o: " + consistencia.split("!@")[2] + "<br>");
                            }
                        }
                    }
                }
                /* *********TESTES ERRO DIGITACAO********* */
                if (!isEmpty(erroDig)) {
                    if (erroDig.indexOf("#") != -1) {
                        for (var i = 0; i < erroDig.split("#").length; i++) {
                            if (erroDig.split("#")[i] != 'null') {
                                erros.push("Limite para mensagem de erro de digitação: " + erroDig.split("#")[i]);
                            }
                        }
                    } else {
                        if (erroDig != 'null') {
                            erros.push("Limite para mensagem de erro de digitação: " + erroDig);
                        }
                    }
                }
                /* *********TESTES LIMITES********* */
                if (!isEmpty(limite)) {
                    if (limite.indexOf("#") != -1) {
                        for (var i = 0; i < limite.split("#").length; i++) {
                            respostaFinalAlert = respostaFinalAlert == "" ? "&bull; Limite: " + limite.split("#")[i] : respostaFinalAlert + "</br> &bull; Limite: " + limite.split("#")[i];
                        }
                    } else {
                        respostaFinalAlert = respostaFinalAlert == "" ? "&bull; Limite: " + limite + "<br/>" : respostaFinalAlert + "</br>  &bull; Limite: " + limite + "<br/>";
                    }
                }
                //Caso tenha alertas na tela, mostra mas passa;
                if (respostaFinalAlert != '') {
                    $('#info').html(respostaFinalAlert);
                    $('#modalCamposDigitados').modal('show');
                }
            }
        }).fail(function (jqXHR, textStatus, errorThrown) {
            alert('Houve problemas ao salvar os campos digitados, erros: ' + 
                erros + ', Status: ' + textStatus + ", exceção: " + errorThrown);
        });
        if (erros.length == 0) {
            console.log('Campos Validados, tudo Ok');
            return true;
        } else {
            console.log('Atencoa: ' + erros);
            $('.btMescla').attr('data-contemErros', true);
            $("#carregando").css('display', 'none');
            var ul = jQuery('body .informarCamposDigitaveis .mensagens-erro ul');
            ul.html("");
            for (i = 0; i < erros.length; i++) {
                var li = ul.append('<li>' + erros[i] + '</li>');
            }
            topoTela();
            jQuery('body .informarCamposDigitaveis .mensagens-erro').show();
            return false;
        }
    };
    function fecharMensagens() {
        jQuery('body .informarCamposDigitaveis .mensagens-erro').hide();
    }

    function incluirProdutos(tipotexto, idModal) {
        idModal = idModal.split("incluiProdutos")[1];
        var paramsProduto = {
            tipotexto: tipotexto,
            requisicao: '9'
        };
        urlCampo = '/editor/mesclagem';
        jQuery.ajax({
            type: 'POST',
            url: urlCampo,
            data: paramsProduto,
            async: false
        }).done(function (ret) {
            if (isEmpty(ret.produtos)) {
                $('#corpoModalProdutos div').append('<p>Nenhum Produto encontrado.</p>');
            } else {
                var lista = [];
                listaCorpoProdutos = [];
                for (var i = 0; i < ret.produtos.produtos.length; i++) {
                    var item = [
                        false,
                        ret.produtos.produtos[i].codprod,
                        ret.produtos.produtos[i].descricao
                    ]
                    var item2 = {
                        codprod: ret.produtos.produtos[i].codprod,
                        descricao: ret.produtos.produtos[i].descricao
                    }
                    lista.push(item);
                    listaCorpoProdutos.push(item2);
                }
                if ($.fn.dataTable.isDataTable('#tableModalProdutos' + idModal)) {
                    table.destroy();
                }
                $('#tableModalProdutos' + idModal).dataTable({
                    'sDom': 'frt<"table-info"lip>',
                    'sPaginationType': 'four_button',
                    "bStateSave": false,
                    "data": lista,
                    "columns": [
                        {'title': 'Selec.', 'sClass': 'text-center selec afina_linha col-prod-selec'},
                        {"title": "Codigo", "sClass": "text-center codprod sorting_1 afina_linha col-prod-codigo"},
                        {"title": "Descricao", "sClass": "descr  sorting_1 afina_linha col-prod-desc"},
                    ],
                    "bFilter": true,
                    "bInfo": true,
                    "height": '330px',
                    "scrollable": 'y',
                    "oLanguage": {
                        "sProcessing": "Processando...",
                        "sLengthMenu": "Mostrar _MENU_ registros",
                        "sZeroRecords": "Não foram encontrados resultados",
                        "sInfo": "Mostrando de _START_ até _END_ de _TOTAL_ registros",
                        "sInfoEmpty": "Mostrando de 0 até 0 de 0 registros",
                        "sInfoFiltered": "(filtrado de _MAX_ registros no total)",
                        "sInfoPostFix": "",
                        "sSearch": "Pesquisar: ",
                        "sUrl": "",
                        "oPaginate": {
                            "sFirst": "Primeiro",
                            "sPrevious": " Anterior",
                            "sNext": " Seguinte",
                            "sLast": " Último"
                        }
                    }, 
                    "aoColumnDefs": [{'bSortable': false, "width": "10%", 'aTargets': [0]}]
                });
                transformaProdutosTextoTooltip(idModal);
                configuraApresentacaoTabelaModal('Produtos', idModal);
            }
        });
        $('#modalProdutos' + idModal).show();
        $('input.chkSelec').removeAttr('checked');
    }

    function incluirCid(tipotexto, idModal) {
        idModal = idModal.split("incluiCid")[1];
        var paramsCid = {
            tipotexto: tipotexto,
            requisicao: '10'
        };
        urlCampo = '/editor/mesclagem';
        jQuery.ajax({
            type: 'POST',
            url: urlCampo,
            data: paramsCid,
            async: false
        }).done(function (ret) {
            if (isEmpty(ret.cid)) {
                $('#corpoModalCid div').append('<p>Nenhum CID encontrado.</p>');
            } else {
                var lista = [];
                listaCorpoCid = [];
                for (var i = 0; i < ret.cid.cid.length; i++) {
                    var item = [
                        false,
                        ret.cid.cid[i].codcid,
                        ret.cid.cid[i].descrcid
                    ]
                    var item2 = {
                        codcid: ret.cid.cid[i].codcid,
                        descrcid: ret.cid.cid[i].descrcid
                    }
                    lista.push(item);
                    listaCorpoCid.push(item2);
                }
                if ($.fn.dataTable.isDataTable('#tableModalCid' + idModal)) {
                    table.destroy();
                }
                $('#tableModalCid' + idModal).dataTable({
                    'sDom': 'frt<"table-info"lip>',
                    'sPaginationType': 'four_button',
                    "bStateSave": false,
                    "data": lista,
                    "columns": [
                        {'title': 'Selec.', 'sClass': 'text-center selec afina_linha col-cid-selec'},
                        {"title": "Codigo", "sClass": "text-center codcid sorting_1 afina_linha col-cid-codigo"},
                        {"title": "Descricao", "sClass": "descr afina_linha sorting_1 col-cid-desc"},
                    ],
                    "bFilter": true,
                    "bInfo": true,
                    "height": '330px',
                    "scrollable": 'y',
                    "oLanguage": {
                        "sProcessing": "Processando...",
                        "sLengthMenu": "Mostrar _MENU_ registros",
                        "sZeroRecords": "Não foram encontrados resultados",
                        "sInfo": "Mostrando de _START_ até _END_ de _TOTAL_ registros",
                        "sInfoEmpty": "Mostrando de 0 até 0 de 0 registros",
                        "sInfoFiltered": "(filtrado de _MAX_ registros no total)",
                        "sInfoPostFix": "",
                        "sSearch": "Pesquisar: ",
                        "sUrl": "",
                        "oPaginate": {
                            "sFirst": "Primeiro",
                            "sPrevious": " Anterior",
                            "sNext": " Seguinte",
                            "sLast": " Último"
                        }
                    }, "aoColumnDefs": [{'bSortable': false, "width": "10%", 'aTargets': [0]}]
                });
                transformaCidTextoTooltip(idModal);
                configuraApresentacaoTabelaModal('Cid', idModal);
            }
        });
        $('#modalCid' + idModal).show();
        $('input.chkSelec').removeAttr('checked');
    }
    
    function incluirDiag(tipotexto, idModal) {
        idModal = idModal.split("incluiDiag")[1];
        var paramsDiag = {
            tipotexto: tipotexto,
            requisicao: '11'
        };
        urlCampo = '/editor/mesclagem';
        jQuery.ajax({
            type: 'POST',
            url: urlCampo,
            data: paramsDiag,
            async: false
        }).done(function (ret) {
            if (isEmpty(ret.diag)) {
                $('#corpoModalDiag div').append('<p>Nenhum CID encontrado.</p>');
            } else {
                var lista = [];
                listaCorpoDiag = [];
                for (var i = 0; i < ret.diag.diag.length; i++) {
                    var item = [
                        false,
                        ret.diag.diag[i].coddiag,
                        ret.diag.diag[i].diagno
                    ]
                    var item2 = {
                        coddiag: ret.diag.diag[i].coddiag,
                        diagno: ret.diag.diag[i].diagno
                    }
                    lista.push(item);
                    listaCorpoDiag.push(item2);
                }
                if ($.fn.dataTable.isDataTable('#tableModalDiag' + idModal)) {
                    table.destroy();
                }
                $('#tableModalDiag' + idModal).dataTable({
                    'sDom': 'frt<"table-info"lip>',
                    'sPaginationType': 'four_button',
                    "bStateSave": false,
                    "data": lista,
                    "columns": [
                        {'title': 'Selec.', 'sClass': 'text-center selec afina_linha col-diag-selec'},
                        {"title": "Codigo", "sClass": "text-center coddiag sorting_1 afina_linha col-diag-codigo"},
                        {"title": "Descricao", "sClass": "descr sorting_1 col-diag-desc"},
                    ],
                    "bFilter": true,
                    "bInfo": true,
                    "height": '330px',
                    "scrollable": 'y',
                    "oLanguage": {
                        "sProcessing": "Processando...",
                        "sLengthMenu": "Mostrar _MENU_ registros",
                        "sZeroRecords": "Não foram encontrados resultados",
                        "sInfo": "Mostrando de _START_ até _END_ de _TOTAL_ registros",
                        "sInfoEmpty": "Mostrando de 0 até 0 de 0 registros",
                        "sInfoFiltered": "(filtrado de _MAX_ registros no total)",
                        "sInfoPostFix": "",
                        "sSearch": "Pesquisar: ",
                        "sUrl": "",
                        "oPaginate": {
                            "sFirst": "Primeiro",
                            "sPrevious": " Anterior",
                            "sNext": " Seguinte",
                            "sLast": " Último"
                        }
                    }, "aoColumnDefs": [{'bSortable': false, "width": "10%", 'aTargets': [0]}]
                });
                transformaDiagTextoTooltip(idModal);
                configuraApresentacaoTabelaModal('Diag', idModal);
            }
        });
        $('#modalDiag' + idModal).show();
        $('input.chkSelec').removeAttr('checked');
    }

    function configuraApresentacaoTabelaModal(tabelaModal, idModal) {
        $('div#tableModal' + tabelaModal + idModal + '_length.dataTables_length select').css('width', '60px;');
        $('div#tableModal' + tabelaModal + idModal + '_length.dataTables_length label').css('margin-top', '0px;');
        $('.dataTables_filter').css('padding-top', '0px;');
                
        $('.form-control.input-sm').css('height', '15px');
        $('.form-control.input-sm').css('display', 'inline-block');
        $('#tableModal' + tabelaModal + idModal + '_filter').css('padding', '0px;');
        $('#tableModal' + tabelaModal + idModal + '_filter').css('width', '100px;');
        $('#tableModal' + tabelaModal + idModal + '_filter label').css('width', '100px;');
        $('#tableModal' + tabelaModal + idModal + '_length.dataTables_length label select').css('width', '60px;');
        $('#tableModal' + tabelaModal + idModal + '_length.dataTables_filter.dataTables_filter').css('padding-top', '0px;');
        $('#tableModal' + tabelaModal + idModal + '_length.dataTables_length').css('top', '-10px;');

        $('.top').css({'background': 'none', 'border': 'none'});
        $('#tableModal' + tabelaModal + idModal + ' thead th').css('text-align', 'center');
        $('#tableModal' + tabelaModal + idModal + '_filter').css({"white-space": "nowrap", 'width': '100%'});
        $('#tableModal' + tabelaModal + idModal + '_filter.form-control.input-sm').css({'margin-left': '0px','height': '15px', "width": "91%"});
        $('.dataTables_length').css({'width': '20%'});
        $('#tableModal' + tabelaModal + idModal + '_paginate').parent().css('margin', '0px 0 5px');
        $('#tableModal' + tabelaModal + idModal + '_paginate button').css('font-size', '11px');
        $('#tableModal' + tabelaModal + idModal + '_filter label').css('width', '100%');
        $('#tableModal' + tabelaModal + idModal + '_filter input').css({'height': '5px;', 'width': '91%;'});
        $('#tableModal' + tabelaModal + idModal + '_length').css({'font-size': '11px', 'position': 'relative', 'top': '-10px'});
        $('#tableModal' + tabelaModal + idModal + '_info').css('font-size', '11px');
        $('#tableModal' + tabelaModal + idModal + '_info').css('margin-left', '0px');
        $('.paginate_enabled_next').css('font-size', '11px');
        $('.paginate_disabled_next').css('font-size', '11px');
        $('.paginate_enabled_previous').css('font-size', '11px');
        $('.paginate_disabled_previous').css('font-size', '11px');
        $('#tableModal' + tabelaModal + idModal + '_length select').removeClass('form-control');
        $('#tableModal' + tabelaModal + idModal + '_length select').removeClass('input-sm');
        $('div#tableModal' + tabelaModal + idModal + '_filter.dataTables_filter').css('padding-top', '0px');
        $('div#corpoModal' + tabelaModal + '.modal-body').css('padding-top', '0px');
        $('div#corpoModal' + tabelaModal + '.modal-body').css('padding-bottom', '0px');
        $('div.modal-header').css('padding-top', '5px');
        $('div.modal-header').css('padding-bottom', '5px');
        $('table#tableModal' + tabelaModal + idModal).css('margin-bottom', '5px');
        $('input[type="search"]').css('width', '91%');
        $('input[type="search"]').keyup(function() {
            chamaAcertaLayoutModal(tabelaModal, idModal);
        })
        $('#tableModal' + tabelaModal + idModal + '_length select').click(function () {
            console.log('muda qtde. de registros por página.');
            chamaAcertaLayoutModal(tabelaModal, idModal);
        });
        $('th').click(function () {
            console.log('botão de classificação ativado...');
            chamaAcertaLayoutModal(tabelaModal, idModal);
        });
        console.log('inicio');
        chamaAcertaLayoutModal(idModal);
        $('.paginate_enabled_next').click(function () {
            chamaAcertaLayoutModal(tabelaModal, idModal);
        });
        $('.paginate_enabled_previous').first().click(function() {
           chamaAcertaLayoutModal(tabelaModal, idModal);
        });
        $('.dataTables_paginate span:nth-child(2)').click(function() {
           console.log('voltar');
           chamaAcertaLayoutModal(tabelaModal, idModal);
        });
        //$('#tableModal' + tabelaModal + idModal).click();
    }

    function chamaAcertaLayoutModal(tabelaModal, idModal) {
        if (tabelaModal == 'Cid') { 
            acertaLayoutModalCid(idModal);
        } else if (tabelaModal == 'Produtos') { 
            acertaLayoutModalProdutos(idModal);
        } else if (tabelaModal == 'Diag') { 
            acertaLayoutModalDiag(idModal);
        } else if (tabelaModal == 'Tabppadr') { 
            acertaLayoutModalTabppadr(idModal);
        } else if (tabelaModal == 'Cadmedic') { 
            acertaLayoutModalCadmedic(idModal);
        } else if (tabelaModal == 'Txtfrase') { 
            acertaLayoutModalTxtfrase(idModal);
        } else if (tabelaModal == 'Tabintsv') { 
            acertaLayoutModalTabintsv(idModal);
        } 
    }
    
    function incluirTabppadr(tipotexto, idModal) {
        idModal = idModal.split("incluiTabppadr")[1];
        var paramsTabppadr = {
            tipotexto: tipotexto,
            requisicao: '12'
        };
        urlCampo = '/editor/mesclagem';
        jQuery.ajax({
            type: 'POST',
            url: urlCampo,
            data: paramsTabppadr,
            async: false
        }).done(function (ret) {
            if (isEmpty(ret.tabppadr)) {
                $('#corpoModalTabppadr div').append('<p>Nenhum Procedimento encontrado.</p>');
            } else {
                var lista = [];
                listaCorpoTabppadr = [];
                for (var i = 0; i < ret.tabppadr.tabppadr.length; i++) {
                    var item = [
                        false,
                        ret.tabppadr.tabppadr[i].codtbppadr,
                        ret.tabppadr.tabppadr[i].codsppadr,
                        ret.tabppadr.tabppadr[i].descrsp,
                    ]
                    var item2 = {
                        codtbppadr: ret.tabppadr.tabppadr[i].codtbppadr,
                        codsppadr: ret.tabppadr.tabppadr[i].codsppadr,
                        descrsp: ret.tabppadr.tabppadr[i].descrsp
                    }
                    lista.push(item);
                    listaCorpoTabppadr.push(item2);
                }
                if ($.fn.dataTable.isDataTable('#tableModalTabppadr' + idModal)) {
                    table.destroy();
                }
                $('#tableModalTabppadr' + idModal).dataTable({
                    'sDom': 'frt<"table-info"lip>',
                    'sPaginationType': 'four_button',
                    "bStateSave": false,
                    "data": lista,
                    "columns": [
                        {'title': 'Selec.', 'sClass': 'text-center selec afina_linha col-tabppadr-selec'},
                        {"title": "Codigo Tabela", "sClass": "text-center codtbppadr sorting_1 afina_linha col-tabppadr-codigo-tabela"},
                        {"title": "Codigo Servico", "sClass": "text-center codsppadr sorting_1 afina_linha col-tabppadr-codigo-servico"},
                        {"title": "Descricao", "sClass": "descr sorting_1 afina_linha col-tabppadr-desc"},
                    ],
                    "bFilter": true,
                    "bInfo": true,
                    "height": '330px',
                    "scrollable": 'y',
                    "oLanguage": {
                        "sProcessing": "Processando...",
                        "sLengthMenu": "Mostrar _MENU_ registros",
                        "sZeroRecords": "Não foram encontrados resultados",
                        "sInfo": "Mostrando de _START_ até _END_ de _TOTAL_ registros",
                        "sInfoEmpty": "Mostrando de 0 até 0 de 0 registros",
                        "sInfoFiltered": "(filtrado de _MAX_ registros no total)",
                        "sInfoPostFix": "",
                        "sSearch": "Pesquisar: ",
                        "sUrl": "",
                        "oPaginate": {
                            "sFirst": "Primeiro",
                            "sPrevious": " Anterior",
                            "sNext": " Seguinte",
                            "sLast": " Último"
                        }
                    }, "aoColumnDefs": [{'bSortable': false, "width": "10%", 'aTargets': [0]}]
                });
                transformaTabppadrTextoTooltip(idModal);
                configuraApresentacaoTabelaModal('Tabppadr', idModal);
            }
        });
        $('#modalTabppadr' + idModal).show();
        $('input.chkSelec').removeAttr('checked');
    }

    function incluirCadmedic(tipotexto, idModal) {
        idModal = idModal.split("incluiCadmedic")[1];
        var paramsCadmedic = {
            tipotexto: tipotexto,
            requisicao: '13'
        };
        urlCampo = '/editor/mesclagem';
        jQuery.ajax({
            type: 'POST',
            url: urlCampo,
            data: paramsCadmedic,
            async: false
        }).done(function (ret) {
            if (isEmpty(ret.cadmedic)) {
                $('#corpoModalCadmedic div').append('<p>Nenhum Nome Comercial encontrado.</p>');
            } else {
                var lista = [];
                listaCorpoCadmedic = [];
                for (var i = 0; i < ret.cadmedic.cadmedic.length; i++) {
                    var item = [
                        false,
                        ret.cadmedic.cadmedic[i].codmedic,
                        ret.cadmedic.cadmedic[i].nomemedic
                    ]
                    var item2 = {
                        codmedic: ret.cadmedic.cadmedic[i].codmedic,
                        nomemedic: ret.cadmedic.cadmedic[i].nomemedic
                    }
                    lista.push(item);
                    listaCorpoCadmedic.push(item2);
                }
                if ($.fn.dataTable.isDataTable('#tableModalCadmedic' + idModal)) {
                    table.destroy();
                }
                $('#tableModalCadmedic' + idModal).dataTable({
                    'sDom': 'frt<"table-info"lip>',
                    'sPaginationType': 'four_button',
                    "bStateSave": false,
                    "data": lista,
                    "columns": [
                        {'title': 'Selec.', 'sClass': 'text-center selec afina_linha col-cadmedic-selec'},
                        {"title": "Codigo", "sClass": "text-center codmedic sorting_1 afina_linha col-cadmedic-codigo"},
                        {"title": "Descricao", "sClass": "descr sorting_1 afina_linha col-cadmedic-desc"},
                    ],
                    "bFilter": true,
                    "bInfo": true,
                    "height": '330px',
                    "scrollable": 'y',
                    "oLanguage": {
                        "sProcessing": "Processando...",
                        "sLengthMenu": "Mostrar _MENU_ registros",
                        "sZeroRecords": "Não foram encontrados resultados",
                        "sInfo": "Mostrando de _START_ até _END_ de _TOTAL_ registros",
                        "sInfoEmpty": "Mostrando de 0 até 0 de 0 registros",
                        "sInfoFiltered": "(filtrado de _MAX_ registros no total)",
                        "sInfoPostFix": "",
                        "sSearch": "Pesquisar: ",
                        "sUrl": "",
                        "oPaginate": {
                            "sFirst": "Primeiro",
                            "sPrevious": " Anterior",
                            "sNext": " Seguinte",
                            "sLast": " Último"
                        }
                    }, "aoColumnDefs": [{'bSortable': false, "width": "10%", 'aTargets': [0]}]
                });
                transformaCadmedicTextoTooltip(idModal);
                configuraApresentacaoTabelaModal('Cadmedic', idModal);
            }
        });
        $('#modalCadmedic' + idModal).show();
        $('input.chkSelec').removeAttr('checked');
    }

    function cadastraTxtfrase(numcampo, frase, id) {
        var idToClose = id.substr(18, id.length);
        var id = 'laudo' + id.substr(18, id.length);
        var fraseTexto = eval("CKEDITOR.instances." + frase + ".getData()");
        if (fraseTexto.trim() == "") {
            alert("A descrição da frase é um campo obrigatório.");
        } else {
            var paramsTxtfrase = {
                numtexto: $('#numtextoRequest').val(),
                numcampo: eval(numcampo),
                frase: fraseTexto,
                requisicao: '18'
            };
            urlCampo = '/editor/mesclagem';
            jQuery.ajax({
                type: 'POST',
                url: urlCampo,
                data: paramsTxtfrase,
                async: false
            }).done(function () {
                eval("CKEDITOR.instances." + id + ".insertHtml(fraseTexto)");
                eval("CKEDITOR.instances." + id + ".insertText('\\n')");
                fecharModalGenerico('#modalTxtfrase' + idToClose);        
            });
        }
    }

    function incluirTxtfrase(tipotexto, idModal, numcampo) {
        var idParteTextoCampo = $('#numtextoRequest').val() + numcampo;
        idModal = idModal.split("incluiTxtfrase")[1];
        var paramsTxtfrase = {
            tipotexto: tipotexto,
            numtexto: $('#numtextoRequest').val(),
            numcampo: numcampo,
            requisicao: '15'
        };
        urlCampo = '/editor/mesclagem';
        jQuery.ajax({
            type: 'POST',
            url: urlCampo,
            data: paramsTxtfrase,
            async: false
        }).done(function (ret) {
            if (isEmpty(ret.txtfrase)) {
                $('#corpoModalTxtfrase div').append('<p>Nenhuma frase encontrado.</p>');
            } else {
                var lista = [];
                listaCorpoTxtfrase = [];
                for (var i = 0; i < ret.txtfrase.txtfrase.length; i++) {
                    var textoTxtfrase = ret.txtfrase.txtfrase[i].frase;
                    var textoTxtfraseReduzida = textoTxtfrase.length > 20 ? textoTxtfrase.substring(0,19) : textoTxtfrase;
                    //ret.txtfrase.txtfrase[i].numcampo,
                    var item = [
                        false,
                        ret.txtfrase.txtfrase[i].codigo, 
                        textoTxtfraseReduzida, 
                        ret.txtfrase.txtfrase[i].frase 
                    ]
                    var item2 = {
                        codigo: ret.txtfrase.txtfrase[i].codigo,
                        numcampo: textoTxtfraseReduzida,
                        frase: ret.txtfrase.txtfrase[i].frase
                    }
                    lista.push(item);
                    listaCorpoTxtfrase.push(item2);
                }
                if ($.fn.dataTable.isDataTable('#tableModalTxtfrase' + idModal)) {
                    $('#tableModalTxtfrase' + idModal).dataTable().fnClearTable();
                    $('#tableModalTxtfrase' + idModal).dataTable().fnDestroy();
                }
                //
                $('#tableModalTxtfrase' + idModal).dataTable({
                    'sDom': 'frt<"table-info"lip>',
                    'sPaginationType': 'four_button',
                    "bStateSave": false,
                    "data": lista,
                    "columns": [
                        {'title': 'Selec.', 'sClass': 'text-center selec afina_linha col-txtfrase-selec'},
                        {"title": "Codigo", "sClass": "text-center codigo sorting_1 afina_linha col-txtfrase-codigo"},
                        {"title": "Frase Reduzida", "sClass": "text-center numcampo sorting_1 afina_linha col-txtfrase-numcampo"},
                        {"title": "Visualizar Frase", "sClass": "frase text-center sorting_1 afina_linha col-txtfrase-desc"},
                    ],
                    "bFilter": true,
                    "bInfo": true,
                    "height": '330px',
                    "scrollable": 'y',
                    "oLanguage": {
                        "sProcessing": "Processando...",
                        "sLengthMenu": "Mostrar _MENU_ registros",
                        "sZeroRecords": "Não foram encontrados resultados",
                        "sInfo": "Mostrando de _START_ até _END_ de _TOTAL_ registros",
                        "sInfoEmpty": "Mostrando de 0 até 0 de 0 registros",
                        "sInfoFiltered": "(filtrado de _MAX_ registros no total)",
                        "sInfoPostFix": "",
                        "sSearch": "Pesquisar: ",
                        "sUrl": "",
                        "oPaginate": {
                            "sFirst": "Primeiro",
                            "sPrevious": " Anterior",
                            "sNext": " Seguinte",
                            "sLast": " Último"
                        }
                    }, "aoColumnDefs": [{'bSortable': false, "width": "10%", 'aTargets': [0]}]
                });
                transformaTxtfraseTextoTooltip(idModal);
                configuraApresentacaoTabelaModal('Txtfrase', idModal);
                ativaConsultaTxtfrase(idParteTextoCampo);
            }
        });
        $('#modalTxtfrase' + idModal).show();
        $('input.chkSelec').removeAttr('checked');
        var txtCompare = 'cadfrase' + $('#numtextoRequest').val() + numcampo;
        for(var instanceName in CKEDITOR.instances) {
            if (CKEDITOR.instances[instanceName].name == txtCompare) {
                CKEDITOR.instances[instanceName].setData("");
            }
        }        
        CKEDITOR.replace($('#cadfrase' + $('#numtextoRequest').val() + numcampo).attr("id"), {
            toolbar: ('Basic2'),
            height: 80,
            startupFocus: false,
            wordcount: {
                showCharCount: true,
	        maxCharCount: 5000 
            }
        });
    }
    
    function incluirTabintsv(tipotexto, idModal) {
        idModal = idModal.split("incluiTabintsv")[1];
        var paramsTabintsv = {
            tipotexto: tipotexto,
            requisicao: '14'
        };
        urlCampo = '/editor/mesclagem';
        jQuery.ajax({
            type: 'POST',
            url: urlCampo,
            data: paramsTabintsv,
            async: false
        }).done(function (ret) {
            if (isEmpty(ret.tabintsv)) {
                $('#corpoModalTabintsv div').append('<p>Nenhum serviço encontrado.</p>');
            } else {
                var lista = [];
                listaCorpoTabintsv = [];
                for (var i = 0; i < ret.tabintsv.tabintsv.length; i++) {
                    var item = [
                        false,
                        ret.tabintsv.tabintsv[i].codintsv,
                        ret.tabintsv.tabintsv[i].descintsv
                    ]
                    var item2 = {
                        codintsv: ret.tabintsv.tabintsv[i].codintsv,
                        descintsv: ret.tabintsv.tabintsv[i].descintsv
                    }
                    lista.push(item);
                    listaCorpoTabintsv.push(item2);
                }
                if ($.fn.dataTable.isDataTable('#tableModalTabintsv' + idModal)) {
                    table.destroy();
                }
                $('#tableModalTabintsv' + idModal).dataTable({
                    'sDom': 'frt<"table-info"lip>',
                    'sPaginationType': 'four_button',
                    "bStateSave": false,
                    "data": lista,
                    "columns": [
                        {'title': 'Selec.', 'sClass': 'text-center selec afina_linha col-tabintsv-selec'},
                        {"title": "Codigo", "sClass": "text-center codintsv sorting_1 afina_linha col-tabintsv-codigo"},
                        {"title": "Descricao", "sClass": "descr sorting_1 afina_linha col-tabintsv-desc"},
                    ],
                    "bFilter": true,
                    "bInfo": true,
                    "height": '330px',
                    "scrollable": 'y',
                    "oLanguage": {
                        "sProcessing": "Processando...",
                        "sLengthMenu": "Mostrar _MENU_ registros",
                        "sZeroRecords": "Não foram encontrados resultados",
                        "sInfo": "Mostrando de _START_ até _END_ de _TOTAL_ registros",
                        "sInfoEmpty": "Mostrando de 0 até 0 de 0 registros",
                        "sInfoFiltered": "(filtrado de _MAX_ registros no total)",
                        "sInfoPostFix": "",
                        "sSearch": "Pesquisar: ",
                        "sUrl": "",
                        "oPaginate": {
                            "sFirst": "Primeiro",
                            "sPrevious": " Anterior",
                            "sNext": " Seguinte",
                            "sLast": " Último"
                        }
                    }, "aoColumnDefs": [{'bSortable': false, "width": "10%", 'aTargets': [0]}]
                });
                transformaTabintsvTextoTooltip(idModal);
                configuraApresentacaoTabelaModal('Tabintsv', idModal);
            }
        });
        $('#modalTabintsv' + idModal).show();
        $('input.chkSelec').removeAttr('checked');
    }
    
    function acertaLayoutModalProdutos(idModal) {
        $('#tableModalProdutos' + idModal + ' tbody .selec').html('<div style="text-align: center;"><input type="checkbox" class="chkSelec"/></div>');
        $('#tableModalProdutos' + idModal + ' thead .selec').removeClass('sorting_asc');
        $('#tableModalProdutos' + idModal + ' tr').css('height', '30px');
        $('input.chkSelec').removeAttr('checked');
        produtosInclusao = [];
        $('.chkSelec').click(function () {
            var check = $(this).is(':checked');
            var codprod = $(this).closest('tr').find('.codprod').html();
            if (check) {
                var item = {
                    order: produtosInclusao.length + 1,
                    codprod: codprod
                }
                produtosInclusao.push(item)
            } else {
                for (var i = 0; i < produtosInclusao.length; i++) {
                    if (codprod == produtosInclusao[i].codprod) {
                        delete produtosInclusao[i];
                        var produtoTemp = [];
                        for (var j = 0; j < produtosInclusao.length; j++) {
                            if (produtosInclusao[j] != null) {
                                var item = {
                                    order: produtoTemp.length + 1,
                                    codprod: produtosInclusao[j].codprod
                                }
                                produtoTemp.push(item);
                            }
                        }
                        produtosInclusao = produtoTemp;
                        break;
                    }
                }
            }
        });
    }

    function acertaLayoutModalCid(idModal) {
        $('#tableModalCid' + idModal + ' tbody .selec').html('<div style="text-align: center;"><input type="checkbox" checked="false" class="chkSelec"/></div>');
        $('#tableModalCid' + idModal + ' thead .selec').removeClass('sorting_asc');
        $('#tableModalCid' + idModal + ' tr').css('height', '30px');
        $('input.chkSelec').removeAttr('checked');
        cidInclusao = [];
        $('.chkSelec').click(function () {
            var check = $(this).is(':checked');
            var codcid = $(this).closest('tr').find('.codcid').html();
            if (check) {
                var item = {
                    order: cidInclusao.length + 1,
                    codcid: codcid
                }
                cidInclusao.push(item)
            } else {
                for (var i = 0; i < cidInclusao.length; i++) {
                    if (codcid == cidInclusao[i].codcid) {
                        delete cidInclusao[i];
                        var cidTemp = [];
                        for (var j = 0; j < cidInclusao.length; j++) {
                            if (cidInclusao[j] != null) {
                                var item = {
                                    order: cidTemp.length + 1,
                                    codcid: cidInclusao[j].codcid
                                }
                                cidTemp.push(item);
                            }
                        }
                        cidInclusao = cidTemp;
                        break;
                    }
                }
            }
        });
    }

    function acertaLayoutModalDiag(idModal) {
        $('#tableModalDiag' + idModal + ' tbody .selec').html('<div style="text-align: center;"><input type="checkbox" checked="false" class="chkSelec" /></div>');
        $('#tableModalDiag' + idModal + ' thead .selec').removeClass('sorting_asc');
        $('#tableModalDiag' + idModal + ' tr').css('height', '30px');
        $('input.chkSelec').removeAttr('checked');
        diagInclusao = [];
        $('.chkSelec').click(function () {
            var check = $(this).is(':checked');
            var coddiag = $(this).closest('tr').find('.coddiag').html();
            if (check) {
                var item = {
                    order: diagInclusao.length + 1,
                    coddiag: coddiag
                }
                diagInclusao.push(item)
            } else {
                for (var i = 0; i < diagInclusao.length; i++) {
                    if (coddiag == diagInclusao[i].coddiag) {
                        delete diagInclusao[i];
                        var diagTemp = [];
                        for (var j = 0; j < diagInclusao.length; j++) {
                            if (diagInclusao[j] != null) {
                                var item = {
                                    order: diagTemp.length + 1,
                                    coddiag: diagInclusao[j].coddiag
                                }
                                diagTemp.push(item);
                            }
                        }
                        diagInclusao = diagTemp;
                        break;
                    }
                }
            }
        });
    }

    function acertaLayoutModalTabppadr(idModal) {
        $('#tableModalTabppadr' + idModal + ' tbody .selec').html('<div style="text-align: center;"><input type="checkbox" checked="false" class="chkSelec"/></div>');
        $('#tableModalTabppadr' + idModal + ' thead .selec').removeClass('sorting_asc');
        $('#tableModalTabppadr' + idModal + ' tr').css('height', '30px');
        $('input.chkSelec').removeAttr('checked');
        tabppadrInclusao = [];
        $('.chkSelec').click(function () {
            var check = $(this).is(':checked');
            var codtbppadr = $(this).closest('tr').find('.codtbppadr').html();
            var codsppadr = $(this).closest('tr').find('.codsppadr').html();
            if (check) {
                var item = {
                    order: tabppadrInclusao.length + 1,
                    codtbppadr: codtbppadr,
                    codsppadr: codsppadr
                }
                tabppadrInclusao.push(item);
            } else {
                for (var i = 0; i < tabppadrInclusao.length; i++) {
                    if (codtbppadr == tabppadrInclusao[i].codtbppadr && codsppadr == tabppadrInclusao[i].codsppadr) {
                        delete tabppadrInclusao[i];
                        var tabppadrTemp = [];
                        for (var j = 0; j < tabppadrInclusao.length; j++) {
                            if (tabppadrInclusao[j] != null) {
                                var item = {
                                    order: tabppadrTemp.length + 1,
                                    codtbppadr: tabppadrInclusao[j].codtbppadr,
                                    codsppadr: tabppadrInclusao[j].codsppadr
                                }
                                tabppadrTemp.push(item);
                            }
                        }
                        tabppadrInclusao = tabppadrTemp;
                        break;
                    }
                }
            }
        });
    }

    function acertaLayoutModalCadmedic(idModal) {
        $('#tableModalCadmedic' + idModal + ' tbody .selec').html('<div style="text-align: center;"><input type="checkbox" checked="false" class="chkSelec"/></div>');
        $('#tableModalCadmedic' + idModal + ' thead .selec').removeClass('sorting_asc');
        $('#tableModalCadmedic' + idModal + ' tr').css('height', '30px');
        $('input.chkSelec').removeAttr('checked');
        cadmedicInclusao = [];
        $('.chkSelec').click(function () {
            var check = $(this).is(':checked');
            var codmedic = $(this).closest('tr').find('.codmedic').html();
            if (check) {
                var item = {
                    order: cadmedicInclusao.length + 1,
                    codmedic: codmedic
                }
                cadmedicInclusao.push(item);
            } else {
                for (var i = 0; i < cadmedicInclusao.length; i++) {
                    if (codmedic == cadmedicInclusao[i].codmedic) {
                        delete cadmedicInclusao[i];
                        var cadmedicTemp = [];
                        for (var j = 0; j < cadmedicInclusao.length; j++) {
                            if (cadmedicInclusao[j] != null) {
                                var item = {
                                    order: cadmedicTemp.length + 1,
                                    codmedic: cadmedicInclusao[j].codmedic
                                }
                                cadmedicTemp.push(item);
                            }
                        }
                        cadmedicInclusao = cadmedicTemp;
                        break;
                    }
                }
            }
        });
    }

    function acertaLayoutModalTabintsv(idModal) {
        $('#tableModalTabintsv' + idModal + ' tbody .selec').html('<div style="text-align: center;"><input type="checkbox" checked="false" class="chkSelec"/></div>');
        $('#tableModalTabintsv' + idModal + ' thead .selec').removeClass('sorting_asc');
        $('#tableModalTabintsv' + idModal + ' tr').css('height', '30px');
        $('input.chkSelec').removeAttr('checked');
        tabintsvInclusao = [];
        $('.chkSelec').click(function () {
            var check = $(this).is(':checked');
            var codintsv = $(this).closest('tr').find('.codintsv').html();
            if (check) {
                var item = {
                    order: tabintsvInclusao.length + 1,
                    codintsv: codintsv
                }
                tabintsvInclusao.push(item);
            } else {
                for (var i = 0; i < tabintsvInclusao.length; i++) {
                    if (codintsv == tabintsvInclusao[i].codintsv) {
                        delete tabintsvInclusao[i];
                        var tabintsvTemp = [];
                        for (var j = 0; j < tabintsvInclusao.length; j++) {
                            if (tabintsvInclusao[j] != null) {
                                var item = {
                                    order: tabintsvTemp.length + 1,
                                    codintsv: tabintsvInclusao[j].codintsv
                                }
                                tabintsvTemp.push(item);
                            }
                        }
                        tabintsvInclusao = tabintsvTemp;
                        break;
                    }
                }
            }
        });
    }

    function acertaLayoutModalTxtfrase(idModal) {
        $('#tableModalTxtfrase' + idModal + ' tbody .selec').html('<div style="text-align: center;"><input type="checkbox" checked="false" class="chkSelec"/></div>');
        $('#tableModalTxtfrase' + idModal + ' thead .selec').removeClass('sorting_asc');
        $('#tableModalTxtfrase' + idModal + ' tr').css('height', '30px');
        $('input.chkSelec').removeAttr('checked');
        txtfraseInclusao = [];
        $('.chkSelec').click(function () {
            var check = $(this).is(':checked');
            var numcampo = $(this).closest('tr').find('.numcampo').html();
            var codigo = $(this).closest('tr').find('.codigo').html();
            if (check) {
                var item = {
                    order: txtfraseInclusao.length + 1,
                    numcampo: numcampo,
                    codigo: codigo
                }
                txtfraseInclusao.push(item);
            } else {
                for (var i = 0; i < txtfraseInclusao.length; i++) {
                    if (numcampo == txtfraseInclusao[i].numcampo && codigo == txtfraseInclusao[i].codigo) {
                        delete txtfraseInclusao[i];
                        var txtfraseTemp = [];
                        for (var j = 0; j < txtfraseInclusao.length; j++) {
                            if (txtfraseInclusao[j] != null) {
                                var item = {
                                    order: txtfraseTemp.length + 1,
                                    numcampo: txtfraseInclusao[j].numcampo,
                                    codigo: txtfraseInclusao[j].codigo,
                                    frase: txtfraseInclusao[j].frase
                                }
                                txtfraseTemp.push(item);
                            }
                        }
                        txtfraseInclusao = txtfraseTemp;
                        break;
                    }
                }
            }
        });
    }

    function incluiProdutosNoTexto(id, tamanhoMaximo) {
        idToClose = id.substr(14, id.length);
        id = 'laudo' + id.substr(14, id.length);

        var total = eval("CKEDITOR.instances." + id + ".getData().length");

        for (var i = 0; i < produtosInclusao.length; i++) {
            for (var j = 0; j < listaCorpoProdutos.length; j++) {
                if (produtosInclusao[i].codprod == listaCorpoProdutos[j].codprod) {
                    produtosTexto = listaCorpoProdutos[j].descricao; 
                    total += produtosTexto.length;
                    break;
                }
            }
        }
        
        alert("Tamanho dos textos selecionados: " + total + " caracteres.");
        if (total > tamanhoMaximo) {
            alert("O número de caracteres ("+ total + ") do texto do tamanho dos itens selecionados supera o limite do campo de (" + tamanhoMaximo  +") caracteres.");
            return; 
        }

        var produtosTexto = "";
        if (produtosInclusao.length == 0) {
            alert('Nenhum produto foi selecionado');
            return;
        } else {
            for (var i = 0; i < produtosInclusao.length; i++) {
                for (var j = 0; j < listaCorpoProdutos.length; j++) {
                    if (produtosInclusao[i].codprod == listaCorpoProdutos[j].codprod) {
                        //produtosTexto = produtosTexto == "" ? listaCorpoProdutos[j].descricao : produtosTexto + "</br>" + listaCorpoProdutos[j].descricao;
                        eval("CKEDITOR.instances." + id + ".insertText(listaCorpoProdutos[j].descricao)");
                        eval("CKEDITOR.instances." + id + ".insertText('\\n')");
                        break;
                    }
                }
            }
            //eval("CKEDITOR.instances." + id + ".setData(CKEDITOR.instances." + id + ".getData() + '</br>' + produtosTexto)");
            //eval("CKEDITOR.instances." + id + ".insertText(produtosTexto)");
            produtosInclusao = [];
            listaTodosProdutos = [];
        }
        //fecharModalGenerico('#' + modalProdutos$campo.acronimo$campo.pk.numTexto);
        fecharModalGenerico('#modalProdutos' + idToClose);
    }

    function incluiCidNoTexto(id, tamanhoMaximo) {
        idToClose = id.substr(9, id.length);
        id = 'laudo' + id.substr(9, id.length);

        var total = eval("CKEDITOR.instances." + id + ".getData().length");

        for (var i = 0; i < cidInclusao.length; i++) {
            for (var j = 0; j < listaCorpoCid.length; j++) {
                if (cidInclusao[i].codcid == listaCorpoCid[j].codcid) {
                    cidTexto = listaCorpoCid[j].codcid + " - " + listaCorpoCid[j].descrcid; 
                    total += cidTexto.length;
                    break;
                }
            }
        }
        
        alert("Tamanho dos textos selecionados: " + total + " caracteres.");
        if (total > tamanhoMaximo) {
            alert("O número de caracteres ("+ total + ") do texto do tamanho dos itens selecionados supera o limite do campo de (" + tamanhoMaximo  +") caracteres.");
            return; 
        }

        var cidTexto = "";
        if (cidInclusao.length == 0) {
            alert('Nenhum cid foi selecionado');
            return;
        } else {
            for (var i = 0; i < cidInclusao.length; i++) {
                for (var j = 0; j < listaCorpoCid.length; j++) {
                    if (cidInclusao[i].codcid == listaCorpoCid[j].codcid) {
                        //cidTexto = cidTexto == "" ? listaCorpoCid[j].codcid + " - " + listaCorpoCid[j].descrcid : cidTexto + "</br>" + listaCorpoCid[j].codcid + " - " + listaCorpoCid[j].descrcid;
                        cidTexto = listaCorpoCid[j].codcid + " - " + listaCorpoCid[j].descrcid;
                        eval("CKEDITOR.instances." + id + ".insertText(cidTexto)");
                        eval("CKEDITOR.instances." + id + ".insertText('\\n')");
                        break;
                    }
                }
            }
            //eval("CKEDITOR.instances." + id + ".insertText(cidTexto)");
            cidInclusao = [];
            listaTodosCid = [];
        }
        fecharModalGenerico('#modalCid' + idToClose);
    }

    function incluiDiagNoTexto(id, tamanhoMaximo) {
        idToClose = id.substr(10, id.length);
        id = 'laudo' + id.substr(10, id.length);

        var total = eval("CKEDITOR.instances." + id + ".getData().length");

        for (var i = 0; i < diagInclusao.length; i++) {
            for (var j = 0; j < listaCorpoDiag.length; j++) {
                    if (diagInclusao[i].coddiag == listaCorpoDiag[j].coddiag) {
                    diagTexto = listaCorpoDiag[j].diagno; 
                    total += diagTexto.length;
                    break;
                }
            }
        }

        
        alert("Tamanho dos textos selecionados: " + total + " caracteres.");
        if (total > tamanhoMaximo) {
            alert("O número de caracteres ("+ total + ") do texto do tamanho dos itens selecionados supera o limite do campo de (" + tamanhoMaximo  +") caracteres.");
            return; 
        }

        var diagTexto = "";
        if (diagInclusao.length == 0) {
            alert('Nenhum diagnóstico foi selecionado');
            return;
        } else {
            for (var i = 0; i < diagInclusao.length; i++) {
                for (var j = 0; j < listaCorpoDiag.length; j++) {
                    if (diagInclusao[i].coddiag == listaCorpoDiag[j].coddiag) {
                        //diagTexto = diagTexto == "" ? listaCorpoDiag[j].diagno : diagTexto + "</br>" + listaCorpoDiag[j].diagno;
                        eval("CKEDITOR.instances." + id + ".insertText(listaCorpoDiag[j].diagno)");
                        eval("CKEDITOR.instances." + id + ".insertText('\\n')");
                        break;
                    }
                }
            }
            //eval("CKEDITOR.instances." + id + ".insertText(diagTexto)");
            diagInclusao = [];
            listaTodosDiag = [];
        }
        fecharModalGenerico('#modalDiag' + idToClose);
    }

    function incluiTabppadrNoTexto(id, tamanhoMaximo) {
        idToClose = id.substr(14, id.length);
        id = 'laudo' + id.substr(14, id.length);

        var total = eval("CKEDITOR.instances." + id + ".getData().length");

        for (var i = 0; i < tabppadrInclusao.length; i++) {
            for (var j = 0; j < listaCorpoTabppadr.length; j++) {
                if (tabppadrInclusao[i].codtbppadr == listaCorpoTabppadr[j].codtbppadr && 
                    tabppadrInclusao[i].codsppadr == listaCorpoTabppadr[j].codsppadr) {
                    tabppadrTexto = listaCorpoTabppadr[j].codsppadr + " - " + listaCorpoTabppadr[j].descrsp; 
                    total += tabppadrTexto.length;
                    break;
                }
            }
        }

        
        alert("Tamanho dos textos selecionados: " + total + " caracteres.");
        if (total > tamanhoMaximo) {
            alert("O número de caracteres ("+ total + ") do texto do tamanho dos itens selecionados supera o limite do campo de (" + tamanhoMaximo  +") caracteres.");
            return; 
        }

        var tabppadrTexto = "";
        if (tabppadrInclusao.length == 0) {
            alert('Nenhum procedimento foi selecionado');
            return;
        } else {
            for (var i = 0; i < tabppadrInclusao.length; i++) {
                for (var j = 0; j < listaCorpoTabppadr.length; j++) {
                    if (tabppadrInclusao[i].codtbppadr == listaCorpoTabppadr[j].codtbppadr && 
                        tabppadrInclusao[i].codsppadr == listaCorpoTabppadr[j].codsppadr) {
                        //tabppadrTexto = tabppadrTexto == "" ? listaCorpoTabppadr[j].codsppadr + " - " + listaCorpoTabppadr[j].descrsp : tabppadrTexto + "</br>" + listaCorpoTabppadr[j].codsppadr + " - " + listaCorpoTabppadr[j].descrsp;
                        tabppadrTexto = listaCorpoTabppadr[j].codsppadr + " - " + listaCorpoTabppadr[j].descrsp; 
                        //eval("CKEDITOR.instances." + id + ".insertText(listaCorpoTabppadr[j].codsppadr + " - " + listaCorpoTabppadr[j].descrsp)");
                        eval("CKEDITOR.instances." + id + ".insertText(tabppadrTexto)");
                        eval("CKEDITOR.instances." + id + ".insertText('\\n')");
                        console.log(eval("CKEDITOR.instances." + id + ".getData()"));
                        console.log(eval("CKEDITOR.instances." + id + ".getData().length"));
                        break;
                    }
                }
            }
            //eval("CKEDITOR.instances." + id + ".insertText(tabppadrTexto)");
            tabppadrInclusao = [];
            listaTodosTabppadr = [];
        }
        fecharModalGenerico('#modalTabppadr' + idToClose);
    }

    function incluiCadmedicNoTexto(id, tamanhoMaximo) {
        idToClose = id.substr(14, id.length);
        id = 'laudo' + id.substr(14, id.length);

        var total = eval("CKEDITOR.instances." + id + ".getData().length");

        for (var i = 0; i < cadmedicInclusao.length; i++) {
            for (var j = 0; j < listaCorpoCadmedic.length; j++) {
                if (cadmedicInclusao[i].codmedic == listaCorpoCadmedic[j].codmedic) {
                    cadmedicTexto = listaCorpoCadmedic[j].nomemedic; 
                    total += cadmedicTexto.length;
                    break;
                }
            }
        }

        
        alert("Tamanho dos textos selecionados: " + total + " caracteres.");
        if (total > tamanhoMaximo) {
            alert("O número de caracteres ("+ total + ") do texto do tamanho dos itens selecionados supera o limite do campo de (" + tamanhoMaximo  +") caracteres.");
            return; 
        }


        var cadmedicTexto = "";
        if (cadmedicInclusao.length == 0) {
            alert('Nenhum nome comercial foi selecionado');
            return;
        } else {
            for (var i = 0; i < cadmedicInclusao.length; i++) {
                for (var j = 0; j < listaCorpoCadmedic.length; j++) {
                    if (cadmedicInclusao[i].codmedic == listaCorpoCadmedic[j].codmedic) {
                        //cadmedicTexto = cadmedicTexto == "" ? listaCorpoCadmedic[j].nomemedic : cadmedicTexto + "</br>" + listaCorpoCadmedic[j].nomemedic;
                        eval("CKEDITOR.instances." + id + ".insertText(listaCorpoCadmedic[j].nomemedic)");
                        eval("CKEDITOR.instances." + id + ".insertText('\\n')");
                        break;
                    }
                }
            }
            //eval("CKEDITOR.instances." + id + ".insertText(cadmedicTexto)");
            cadmedicInclusao = [];
            listaTodosCadmedic = [];
        }
        fecharModalGenerico('#modalCadmedic' + idToClose);
    }

    function incluiTabintsvNoTexto(id, tamanhoMaximo) {
        idToClose = id.substr(14, id.length);
        id = 'laudo' + id.substr(14, id.length);

        var total = eval("CKEDITOR.instances." + id + ".getData().length");

        for (var i = 0; i < tabintsvInclusao.length; i++) {
            for (var j = 0; j < listaCorpoTabintsv.length; j++) {
                if (tabintsvInclusao[i].codintsv == listaCorpoTabintsv[j].codintsv) {
                    tabintsvTexto = listaCorpoTabintsv[j].descintsv; 
                    total += tabintsvTexto.length;
                    break;
                }
            }
        }

        
        alert("Tamanho dos textos selecionados: " + total + " caracteres.");
        if (total > tamanhoMaximo) {
            alert("O número de caracteres ("+ total + ") do texto do tamanho dos itens selecionados supera o limite do campo de (" + tamanhoMaximo  +") caracteres.");
            return; 
        }

        var tabintsvTexto = "";
        if (tabintsvInclusao.length == 0) {
            alert('Nenhum serviço foi selecionado');
            return;
        } else {
            for (var i = 0; i < tabintsvInclusao.length; i++) {
                for (var j = 0; j < listaCorpoTabintsv.length; j++) {
                    if (tabintsvInclusao[i].codintsv == listaCorpoTabintsv[j].codintsv) {
                        //tabintsvTexto = tabintsvTexto == "" ? listaCorpoTabintsv[j].descintsv : tabintsvTexto + "</br>" + listaCorpoTabintsv[j].descintsv;
                        eval("CKEDITOR.instances." + id + ".insertText(listaCorpoTabintsv[j].descintsv)");
                        eval("CKEDITOR.instances." + id + ".insertText('\\n')");
                        break;
                    }
                }
            }
            //eval("CKEDITOR.instances." + id + ".insertText(tabintsvTexto)");
            tabintsvInclusao = [];
            listaTodosTabintsv = [];
        }
        fecharModalGenerico('#modalTabintsv' + idToClose);
    }

    function alternaListaEhCadastroTxtFrase(parteDoId) {
	if ($("#cadastroFraseContainer"+parteDoId).css('display') == 'none') {
            ativaCadastroTxtfrase(parteDoId);
	} else {
            ativaConsultaTxtfrase(parteDoId);
        }
    }

    function ativaCadastroTxtfrase(parteDoId) {
        $("#listaFraseContainer"+parteDoId).css("display", "none");
	$("#cadastroFraseContainer"+parteDoId).css("display", "block");
    }

    function ativaConsultaTxtfrase(parteDoId) {
	$("#cadastroFraseContainer"+parteDoId).css("display", "none");
	$("#listaFraseContainer"+parteDoId).css("display", "block");
    }

    function cadastraFraseNoTexto(frase) {
        alert(eval("CKEDITOR.instances." + frase + ".getData()"));
    }

    function incluiTxtfraseNoTexto(id, tamanhoMaximo) {
        idToClose = id.substr(14, id.length);
        id = 'laudo' + id.substr(14, id.length);

        var total = eval("CKEDITOR.instances." + id + ".getData().length");

        for (var i = 0; i < txtfraseInclusao.length; i++) {
            for (var j = 0; j < listaCorpoTxtfrase.length; j++) {
                if (txtfraseInclusao[i].codigo == listaCorpoTxtfrase[j].codigo) {
                    txtfraseTexto = listaCorpoTxtfrase[j].frase; 
                    total += txtfraseTexto.length;
                    break;
                }
            }
        }
        
        alert("Tamanho dos textos selecionados: " + total + " caracteres.");
        if (total > tamanhoMaximo) {
            alert("O número de caracteres ("+ total + ") do texto do tamanho dos itens selecionados supera o limite do campo de (" + tamanhoMaximo  +") caracteres.");
            return; 
        }

        console.log('incluiTxtfraseNoTexto' + id);
        var txtfraseTexto = "";
        if (txtfraseInclusao.length == 0) {
            alert('Nenhuma frase foi selecionada');
            return;
        } else {
            for (var i = 0; i < txtfraseInclusao.length; i++) {
                for (var j = 0; j < listaCorpoTxtfrase.length; j++) {
                    //if (txtfraseInclusao[i].numcampo == listaCorpoTxtfrase[j].numcampo && 
                    //    txtfraseInclusao[i].codigo == listaCorpoTxtfrase[j].codigo) {
                    console.log(txtfraseInclusao[i].codigo);
                    console.log(listaCorpoTxtfrase[j].codigo);
                    console.log(txtfraseInclusao[i].codigo == listaCorpoTxtfrase[j].codigo);
                    if (txtfraseInclusao[i].codigo == listaCorpoTxtfrase[j].codigo) {
                        //txtfraseTexto = txtfraseTexto == "" ? listaCorpoTxtfrase[j].frase : txtfraseTexto + "</br>" + listaCorpoTxtfrase[j].frase;
                        //eval("CKEDITOR.instances." + id + ".insertText(listaCorpoTxtfrase[j].frase)");
                        eval("CKEDITOR.instances." + id + ".insertHtml(listaCorpoTxtfrase[j].frase)");
                        eval("CKEDITOR.instances." + id + ".insertText('\\n')");
                        break;
                    }
                }
            }
            //eval("CKEDITOR.instances." + id + ".setData(CKEDITOR.instances." + id + ".getData() + '</br>' + txtfraseTexto)");
            txtfraseInclusao = [];
            listaTodosTxtfrase = [];
        }
        fecharModalGenerico('#modalTxtfrase' + idToClose);
    }


     function incluirLaudos(tipotexto, idModal) {
        idModal = idModal.split("incluiLaudos")[1];
        var operadorLogado = retornaValorUrlGet('operadorLogado');
        var paramsLaudo = {
            tipotexto: tipotexto,
            requisicao: '4',
            operadorLogado: operadorLogado
        };
        urlCampo = '/editor/mesclagem';
        jQuery.ajax({
            type: 'POST',
            url: urlCampo,
            data: paramsLaudo,
            async: false
        }).done(function (ret) {
            if (isEmpty(ret.laudos.laudos)) {
                $('.msgNaoEncontrado').remove();
                $('#tableModalLaudos' + idModal + '_wrapper').hide();
                $('#corpoModalLaudos').append('<p class="msgNaoEncontrado">Nenhum Laudo encontrado para este tipo de texto.</p>');
            } else {
                $('.msgNaoEncontrado').remove();
                $('#tableModalLaudos' + idModal + '_wrapper').show();
                var lista = [];
                for (var i = 0; i < ret.laudos.laudos.length; i++) {
                    var item = [
                        false,
                        ret.laudos.laudos[i].numtexto,
                        ret.laudos.laudos[i].nometexto,
                        ret.laudos.laudos[i].corpo
                    ]
                    var item2 = {
                        numtexto: ret.laudos.laudos[i].numtexto,
                        corpo: ret.laudos.laudos[i].corpo
                    }
                    lista.push(item);
                    listaCorpoLaudos.push(item2);
                }
                if ($.fn.dataTable.isDataTable('#tableModalLaudos' + idModal)) {
                    table.destroy();
                }
                $('#tableModalLaudos' + idModal).dataTable({
                    "pagingType": "full_numbers",
                    'sDom': '<"top"f>rt<"table-info"lip>',
                    "data": lista,
                    "columns": [
                        {'title': 'Selec.', 'sClass': 'text-center selec afina_linha col-laudos-selec'},
                        {"title": "Texto", "sClass": "text-center numtexto sorting_1 afina_linha col-laudos-numtexto"},
                        {"title": "Descricao", "sClass": "descr sorting_1 afina_linha col-laudos-desc"},
                        {"title": "Visualizar Laudo", "sClass": "laudo text-center sorting_1 afina_linha col-laudos-visual"},
                    ],
                    "bFilter": true,
                    "paging": false,
                    "bInfo": true,
                    "height": '630px',
                    "scrollable": 'y',
                    "oLanguage": {
                        "sProcessing": "Processando...",
                        "sLengthMenu": "Mostrar _MENU_ registros",
                        "sZeroRecords": "Não foram encontrados resultados",
                        "sInfo": "Mostrando de _START_ até _END_ de _TOTAL_ registros",
                        "sInfoEmpty": "Mostrando de 0 até 0 de 0 registros",
                        "sInfoFiltered": "(filtrado de _MAX_ registros no total)",
                        "sInfoPostFix": "",
                        "sSearch": "Pesquisar: ",
                        "sUrl": "",
                        "oPaginate": {
                            "sFirst": "Primeiro",
                            "sPrevious": "Anterior",
                            "sNext": "Seguinte",
                            "sLast": "Último"
                        }
                    }, "aoColumnDefs": [{'bSortable': false, "width": "10%", 'aTargets': [0]}]
                });
                transformaLaudosTextoTooltip(idModal);
                $('.top').css({'background': 'none', 'border': 'none'});
                $('#tableModalLaudos' + idModal + ' thead th').css('text-align', 'center');
                $('#tableModalLaudos' + idModal + '_filter').css({"white-space": "nowrap", 'width': '100%'});
                $('#tableModalLaudos' + idModal + '_filter input').css({'margin-left': '0px','height': '15px', "width": "99%"});
                $('#tableModalLaudos' + idModal + '_paginate').parent().css('margin', '25px 0 10px');
                $('#tableModalLaudos' + idModal + '_paginate button').css('font-size', '11px');
                $('#tableModalLaudos' + idModal + '_filter label').css('width', '100%');
                $('#tableModalLaudos' + idModal + '_filter input').css({'height': '5px;'});
                $('#tableModalLaudos' + idModal + '_length').css({'font-size': '11px', 'position': 'relative'});
                $('#tableModalLaudos' + idModal + '_info').css('font-size', '11px');
                $('#tableModalLaudos' + idModal + '_info').css('margin-left', '0px');
                acertaLayoutModal(idModal);
                $('.chkSelec').click(function () {
                    var check = $(this).is(':checked');
                    var numtexto = $(this).closest('tr').find('.numtexto').html();
                    if (check) {
                        var item = {
                            order: laudosInclusao.length + 1,
                            numtexto: numtexto
                        }
                        laudosInclusao.push(item)
                    } else {
                        for (var i = 0; i < laudosInclusao.length; i++) {
                            if (numtexto == laudosInclusao[i].numtexto) {
                                delete laudosInclusao[i];
                                var laudoTemp = [];
                                for (var j = 0; j < laudosInclusao.length; j++) {
                                    if (laudosInclusao[j] != null) {
                                        var item = {
                                            order: laudoTemp.length + 1,
                                            numtexto: laudosInclusao[j].numtexto
                                        }
                                        laudoTemp.push(item);
                                    }
                                }
                                laudosInclusao = laudoTemp;
                                break;
                            }
                        }
                    }
                });
            }
            var modalElem = $('#modalLaudos' + idModal);
            modalElem.show();
        });
    }
    function acertaLayoutModal(idModal) {
        $('#tableModalLaudos' + idModal + ' tbody .selec').html('<div style="text-align: center;"><input type="checkbox" class="chkSelec"/></div>');
        $('#tableModalLaudos' + idModal + ' thead .selec').removeClass('sorting_asc');
        $('#tableModalLaudos' + idModal + ' tr').css('height', '30px');
    }

    function incluiLaudosNoTexto(id, tamanhoMaximo) {
        idToClose = id.substr(12, id.length);
        id = 'laudo' + id.substr(12, id.length);

        var total = eval("CKEDITOR.instances." + id + ".getData().length");

        for (var i = 0; i < laudosInclusao.length; i++) {
            for (var j = 0; j < listaCorpoLaudos.length; j++) {
                if (laudosInclusao[i].numtexto == listaCorpoLaudos[j].numtexto) {
                    laudosTexto = listaCorpoLaudos[j].corpo; 
                    total += laudosTexto.length;
                    break;
                }
            }
        }

        
        alert("Tamanho dos textos selecionados: " + total + " caracteres.");
        if (total > tamanhoMaximo) {
            alert("O número de caracteres ("+ total + ") do texto do tamanho dos itens selecionados supera o limite do campo de (" + tamanhoMaximo  +") caracteres.");
            return; 
        }

        var laudosTexto = "";
        if (laudosInclusao.length == 0) {
            alert('Nenhum laudo foi selecionado');
            return;
        } else {
            for (var i = 0; i < laudosInclusao.length; i++) {
                for (var j = 0; j < listaCorpoLaudos.length; j++) {
                    if (laudosInclusao[i].numtexto == listaCorpoLaudos[j].numtexto) {
                        laudosTexto = laudosTexto == "" ? listaCorpoLaudos[j].corpo : laudosTexto + "</br>" + listaCorpoLaudos[j].corpo;
                        break;
                    }
                }
            }
            eval("CKEDITOR.instances." + id + ".setData(CKEDITOR.instances." + id + ".getData() + '</br>' + laudosTexto)");
            laudosInclusao = [];
            listaTodosLaudos = [];
        }
        fecharModalGenerico('#modalLaudos' + idToClose);
    }

    function substituirLaudosNoTexto(id) {
        limparTela('limpa' + id.split('incluiLaudos')[1]);
        setTimeout(function () {
            incluiLaudosNoTexto(id);
        }, 100);
    }

    function isEmpty(obj) {
        for (var prop in obj) {
            if (obj.hasOwnProperty(prop))
                return false;
        }
        return true;
    }

    function limparTela(id) {
        id = id.replace("limpa", "");
        eval(" CKEDITOR.instances." + "laudo" + id + ".setData('') ");
    }

    function fecharModalLaudos(idModal) {
        jQuery(idModal).modal('hide');
    }

    function fecharModalGenerico(idModal) {
        jQuery(idModal).modal('hide');
    }

    //    function cancelaModalLaudos(idModal) {
    //        if (idModal.indexOf("cancel") !== -1) {
    //            idModal = idModal.substring(7, idModal.length);
    //        }
    //        if (!($('#tableModalLaudos' + idModal).is(':empty'))) {
    //            $("#tableModalLaudos" + idModal).dataTable().fnDestroy();
    //            $("#tableModalLaudos" + idModal).empty();
    //        }
    //        $('#modalLaudos').modal('hide');
    //    }

    function transformaLaudosTextoTooltip(idModal) {
        $('#tableModalLaudos' + idModal + ' tbody tr').each(function () { // Percorre a tabela inteira
            var laudo = $(this).find('.laudo');
            var descr = $(this).find('.descr').html();
            var textoLaudo = laudo.html();
            laudo.empty();
            laudo.append('<div class="popover-content"><button type="button" class="close botao-info btTabela" data-trigger="focus" data-toggle="popover" data-placement="bottom" data-container="body" overflow: "visible"><i class="fa fa-info-circle"></i></button></div>');
            $(this).find('.laudo button').attr('data-content', textoLaudo);
            $(this).find('.laudo button').attr('title', descr);
            $(this).find('.laudo div button').popover({html: true, placement: 'bottom', trigger: 'focus'});
            $(this).find('.laudo div button').focus(function () {
                $('.popover-title').css({'font-size': '17px', 'font-weight': 'bold', 'text-transform': 'uppercase'});
                $('.popover').css({'height': '40%', 'min-width': '600px', 'overflow-y': 'scroll'});
            });
            console.log('Início Laudos');
            acertaLayoutModal(idModal);
        });
    }

    function transformaProdutosTextoTooltip(idModal) {
        $('#tableModalProdutos' + idModal + ' tbody tr').each(function () { // Percorre a tabela inteira
            var produto = $(this).find('.produto');
            var descr = $(this).find('.descr').html();
            var textoProduto = produto.html();
            produto.empty();
            produto.append('<div class="popover-content"><button type="button" class="close botao-info btTabela" data-trigger="focus" data-toggle="popover" data-placement="bottom" data-container="body" overflow: "visible"><span class="fa fa-info-circle" style="font-family: Glyphicons Halflings!important"></span></button></div>');
            $(this).find('.produto button').attr('data-content', textoProduto);
            $(this).find('.produto button').attr('title', descr);
            $(this).find('.produto div button').popover({html: true, placement: 'bottom', trigger: 'focus'});
            $(this).find('.produto div button').focus(function () {
                $('.popover-title').css({'font-size': '17px', 'font-weight': 'bold', 'text-transform': 'uppercase'});
                $('.popover').css({'height': '40%', 'min-width': '600px', 'overflow-y': 'scroll'});
            });
            console.log('Início Produtos');
            acertaLayoutModalProdutos(idModal);
        });
    }

    function transformaCidTextoTooltip(idModal) {
        $('#tableModalCid' + idModal + ' tbody tr').each(function () { // Percorre a tabela inteira
            var cid = $(this).find('.cid');
            var descr = $(this).find('.descr').html();
            var textoCid = cid.html();
            cid.empty();
            cid.append('<div class="popover-content"><button type="button" class="close botao-info btTabela" data-trigger="focus" data-toggle="popover" data-placement="bottom" data-container="body" overflow: "visible"><span class="fa fa-info-circle" style="font-family: Glyphicons Halflings!important"></span></button></div>');
            $(this).find('.cid button').attr('data-content', textoCid);
            $(this).find('.cid button').attr('title', descr);
            $(this).find('.cid div button').popover({html: true, placement: 'bottom', trigger: 'focus'});
            $(this).find('.cid div button').focus(function () {
                $('.popover-title').css({'font-size': '17px', 'font-weight': 'bold', 'text-transform': 'uppercase'});
                $('.popover').css({'height': '40%', 'min-width': '600px', 'overflow-y': 'scroll'});
            });
            console.log('Início Cid');
            acertaLayoutModalCid(idModal);
        });
    }

    function transformaDiagTextoTooltip(idModal) {
        $('#tableModalDiag' + idModal + ' tbody tr').each(function () { // Percorre a tabela inteira
            var diag = $(this).find('.diag');
            var descr = $(this).find('.descr').html();
            var textoDiag = diag.html();
            diag.empty();
            diag.append('<div class="popover-content"><button type="button" class="close botao-info btTabela" data-trigger="focus" data-toggle="popover" data-placement="bottom" data-container="body" overflow: "visible"><span class="fa fa-info-circle" style="font-family: Glyphicons Halflings!important"></span></button></div>');
            $(this).find('.diag button').attr('data-content', textoDiag);
            $(this).find('.diag button').attr('title', descr);
            $(this).find('.diag div button').popover({html: true, placement: 'bottom', trigger: 'focus'});
            $(this).find('.diag div button').focus(function () {
                $('.popover-title').css({'font-size': '17px', 'font-weight': 'bold', 'text-transform': 'uppercase'});
                $('.popover').css({'height': '40%', 'min-width': '600px', 'overflow-y': 'scroll'});
            });
            console.log('Início Diagnóstico');
            acertaLayoutModalDiag(idModal);
        });
    }

    function transformaTabppadrTextoTooltip(idModal) {
        $('#tableModalTabppadr' + idModal + ' tbody tr').each(function () { // Percorre a tabela inteira
            var tabppadr = $(this).find('.tabppadr');
            var descr = $(this).find('.descr').html();
            var textoTabppadr = tabppadr.html();
            tabppadr.empty();
            tabppadr.append('<div class="popover-content"><button type="button" class="close botao-info btTabela" data-trigger="focus" data-toggle="popover" data-placement="bottom" data-container="body" overflow: "visible"><span class="fa fa-info-circle" style="font-family: Glyphicons Halflings!important"></span></button></div>');
            $(this).find('.tabppadr button').attr('data-content', textoTabppadr);
            $(this).find('.tabppadr button').attr('title', descr);
            $(this).find('.tabppadr div button').popover({html: true, placement: 'bottom', trigger: 'focus'});
            $(this).find('.tabppadr div button').focus(function () {
                $('.popover-title').css({'font-size': '17px', 'font-weight': 'bold', 'text-transform': 'uppercase'});
                $('.popover').css({'height': '40%', 'min-width': '600px', 'overflow-y': 'scroll'});
            });
            console.log('Início Procedimentos');
            acertaLayoutModalTabppadr(idModal);
        });
    }

    function transformaCadmedicTextoTooltip(idModal) {
        $('#tableModalCadmedic' + idModal + ' tbody tr').each(function () { // Percorre a tabela inteira
            var cadmedic = $(this).find('.cadmedic');
            var descr = $(this).find('.descr').html();
            var textoCadmedic = cadmedic.html();
            cadmedic.empty();
            cadmedic.append('<div class="popover-content"><button type="button" class="close botao-info btTabela" data-trigger="focus" data-toggle="popover" data-placement="bottom" data-container="body" overflow: "visible"><span class="fa fa-info-circle" style="font-family: Glyphicons Halflings!important"></span></button></div>');
            $(this).find('.cadmedic button').attr('data-content', textoCadmedic);
            $(this).find('.cadmedic button').attr('title', descr);
            $(this).find('.cadmedic div button').popover({html: true, placement: 'bottom', trigger: 'focus'});
            $(this).find('.cadmedic div button').focus(function () {
                $('.popover-title').css({'font-size': '17px', 'font-weight': 'bold', 'text-transform': 'uppercase'});
                $('.popover').css({'height': '40%', 'min-width': '600px', 'overflow-y': 'scroll'});
            });
            console.log('Início Nomes Comerciais');
            acertaLayoutModalCadmedic(idModal);
        });
    }

    function transformaTabintsvTextoTooltip(idModal) {
        $('#tableModalTabintsv' + idModal + ' tbody tr').each(function () { // Percorre a tabela inteira
            var tabintsv = $(this).find('.tabintsv');
            var descr = $(this).find('.descr').html();
            var textoTabintsv = tabintsv.html();
            tabintsv.empty();
            tabintsv.append('<div class="popover-content"><button type="button" class="close botao-info btTabela" data-trigger="focus" data-toggle="popover" data-placement="bottom" data-container="body" overflow: "visible"><span class="fa fa-info-circle" style="font-family: Glyphicons Halflings!important"></span></button></div>');
            $(this).find('.tabintsv button').attr('data-content', textoTabintsv);
            $(this).find('.tabintsv button').attr('title', descr);
            $(this).find('.tabintsv div button').popover({html: true, placement: 'bottom', trigger: 'focus'});
            $(this).find('.tabintsv div button').focus(function () {
                $('.popover-title').css({'font-size': '17px', 'font-weight': 'bold', 'text-transform': 'uppercase'});
                $('.popover').css({'height': '40%', 'min-width': '600px', 'overflow-y': 'scroll'});
            });
            console.log('Início Serviços');
            acertaLayoutModalTabintsv(idModal);
        });
    }

    function transformaTxtfraseTextoTooltip(idModal) {
        $('#tableModalTxtfrase' + idModal + ' tbody tr').each(function () { // Percorre a tabela inteira
            var txtfrase = $(this).find('.frase');
            var descr = $(this).find('.codigo').html();
            var textoTxtfrase = txtfrase.html();
            txtfrase.empty();
            txtfrase.append('<div class="popover-content"><button type="button" class="close botao-info btTabela" data-trigger="focus" data-toggle="popover" data-placement="bottom" data-container="body" overflow: "visible"><i class="fa fa-info-circle"></i></button></div>');
            $(this).find('.frase button').attr('data-content', textoTxtfrase);
            $(this).find('.frase button').attr('title', descr);
            $(this).find('.frase div button').popover({html: true, placement: 'bottom', trigger: 'focus'});
            $(this).find('.frase div button').focus(function () {
                $('.popover-title').css({'font-size': '17px', 'font-weight': 'bold', 'text-transform': 'uppercase'});
                $('.popover').css({'height': '40%', 'min-width': '600px', 'overflow-y': 'scroll'});
            });
            console.log('Início Frases');
            acertaLayoutModalTxtfrase(idModal);
        });
    }

    function retornaValorUrlGet(valor) {
        var url = window.location.href;
        if (url.split(valor).length > 1 && url.split(valor)[1].split('&').length > 1) {
            return url.split(valor)[1].split('&')[0].replace('=', '');
        } else {
            return null;
        }
    }

    function StringBuffer() {
        this.buffer = [];
    }
    StringBuffer.prototype.append = function append(string) {
        this.buffer.push(string);
        return this;
    };
    StringBuffer.prototype.toString = function toString() {
        return this.buffer.join("");
    };

</script>
