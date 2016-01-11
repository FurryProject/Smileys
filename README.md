// ==UserScript==
// @name         Furry Project Smileys
// @namespace    https://github.com/FurryProject/Smileys
// @version      0.1
// @author       FurryProject
// @match        http://atelier801.com/*
// @grant        none
// ==/UserScript==

(function() {
		if (document.querySelector("#outils_message_reponse") !== null && document.querySelector("#outils_message_reponse") !== undefined) {
			var parent = document.querySelector("#outils_message_reponse > .btn-group:nth-last-child(2)");
			var bloc = "message_reponse";
		}
		else if (document.querySelector("#outils_message_sujet") !== null && document.querySelector("#outils_message_sujet") !== undefined) {
			var parent = document.querySelector("#outils_message_sujet > .btn-group:nth-last-child(2)");
			var bloc = "message_sujet";
		}
		else if (document.querySelector("#outils_message_conversation") !== null && document.querySelector("#outils_message_conversation") !== undefined) {
			var parent = document.querySelector("#outils_message_conversation > .btn-group:nth-last-child(2)");
			var bloc = "message_conversation";
		}
		else if (document.querySelector("#outils_presentation") !== null && document.querySelector("#outils_presentation") !== undefined) {
			
			var parent = document.querySelector("#outils_presentation > .btn-group:nth-last-child(2)");
			var bloc = "presentation";
		}
		if (parent !== undefined && parent !== null) {
			var node = document.createElement("div");
			node.className = "btn-group groupe-boutons-barre-outils";
			node.innerHTML = "<button type='button' class='btn btn-reduit' title='Smiley FP'><img src='http://i.imgur.com/wVkPOim.png'/></button><button class='btn btn-reduit dropdown-toggle' data-toggle='dropdown'> <span class='caret'></span></button><ul class='dropdown-menu pull-right label-message'> <table style='min-width:300px'> <tbody> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/JH4Zyzx.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/JH4Zyzx.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/nfeZNUt.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/nfeZNUt.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/ZFVWc7B.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/ZFVWc7B.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/DbxeD7z.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/DbxeD7z.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/so4ja.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/so4ja.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/20DUU.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/20DUU.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/lliSm.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/lliSm.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/6z7vx.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/6z7vx.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/dUgHq.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/dUgHq.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/7TTSk.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/7TTSk.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/UWRr0GJ.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/UWRr0GJ.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/8vcM6SC.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/8vcM6SC.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/1W100Wq.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/1W100Wq.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/p6AInvY.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/p6AInvY.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/aTwU9Kt.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/aTwU9Kt.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/cQh0ouT.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/cQh0ouT.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/bFuyN6p.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/bFuyN6p.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/36MbmHc.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/36MbmHc.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/xnVu4sa.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/xnVu4sa.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/m3PRUXO.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/m3PRUXO.png'/></a></li></td></tr></tbody></table></ul>";			parent.parentNode.insertBefore(node, parent.nextSibling);
			parent.parentNode.insertBefore(node, parent.nextSibling);

			node = document.createElement("div");
			node.className = "btn-group groupe-boutons-barre-outils";
			node.innerHTML = "<button type='button' class='btn btn-reduit' title='Smiley Fxie'><img src='http://i.imgur.com/EQaZwCU.png'/></button><button class='btn btn-reduit dropdown-toggle' data-toggle='dropdown'> <span class='caret'></span> </button><ul class='dropdown-menu pull-right label-message'> <table style='min-width:400px'> <tbody> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/Pp8ML.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/Pp8ML.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/QsLNX.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/QsLNX.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/HNQ3Y.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/HNQ3Y.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/qJIDs.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/qJIDs.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/Mn8jf.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/Mn8jf.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/GEW50.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/GEW50.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/MGVC4.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/MGVC4.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/oxVfm.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/oxVfm.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/Opgj5.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/Opgj5.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/SJY1r.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/SJY1r.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/DLTl5.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/DLTl5.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/mjxvy.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/mjxvy.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/obJdw.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/obJdw.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/hHOal.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/hHOal.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/lXve6.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/lXve6.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/5meym.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/5meym.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/0dXU1.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/0dXU1.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/gqvWp.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/gqvWp.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/fRe8E.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/fRe8E.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/JDqoG.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/JDqoG.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/t91LB.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/t91LB.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/WXz5q.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/WXz5q.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/uCfkP.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/uCfkP.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/61uC7.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/61uC7.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/FCJlP.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/FCJlP.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/7pEGa.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/7pEGa.png'/></a></li></td></tr></tbody></table></ul>";
			parent.parentNode.insertBefore(node, parent.nextSibling);

node = document.createElement("div");
node.className = "btn-group groupe-boutons-barre-outils";
node.innerHTML = "<button type='button' class='btn btn-reduit' title='Smileys criados por usuários'><img src='http://atelier801.com/img/icones/16/1historique-posts2.png'/></button><button class='btn btn-reduit dropdown-toggle' data-toggle='dropdown'> <span class='caret'></span> </button><ul class='dropdown-menu pull-right label-message'> <table style='min-width:400px'> <tbody> <tr> <td class='cellule-dropdown'><li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/rTgnFII.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/rTgnFII.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/Eph1x9h.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/Eph1x9h.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/W65lnia.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/W65lnia.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/xNxz3bn.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/xNxz3bn.png'/></a></li> </tr> <tr> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/ZC85E9M.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/ZC85E9M.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/T0NCaJ5.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/T0NCaJ5.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/FXjBjkM.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/FXjBjkM.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/2KiwTyJ.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/2KiwTyJ.png'/></a></li> </td> <tr></tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/X1ix6lN.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/X1ix6lN.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/1UJfPiQ.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/1UJfPiQ.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/Dzmftko.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/Dzmftko.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/5ge1vDG.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/5ge1vDG.png'/></a></li> </td> <tr> </tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/u8iGizM.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/u8iGizM.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/2ebX02S.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/2ebX02S.png'/></a></li> </td> </td></tr></tbody></table></ul>";
parent.parentNode.insertBefore(node, parent.nextSibling);


node = document.createElement("div");
node.className = "btn-group groupe-boutons-barre-outils";
node.innerHTML = "<button type='button' class='btn btn-reduit' title='Créditos'><img src='http://atelier801.com/img/pays/br.png'/></button><button class='btn btn-reduit dropdown-toggle' data-toggle='dropdown'> <span class='caret'></span> </button><ul class='dropdown-menu pull-right label-message'> <table style='min-width:400px'> <tbody> <tr> <td class='cellule-dropdown'><b>Criador</b>: Mcfloy<br><b>Tópico BR</b>: Dedavii<br><b>Smileys</b>: Melibellule, Fxie, Mrkurt, Xtayyguerleo, Doritosgotos<br><br>Atualizado 29/12 - Versão 1.0.1</td></tr></tbody></table></ul>";
parent.parentNode.insertBefore(node, parent.nextSibling);
		}
		var forms = document.querySelectorAll("form[action='edit-topic-message']");
		if (forms !== undefined) {
			for (var i = 0; i < forms.length; i++) {
				var id = forms[i].querySelector("input[name='m']").value;
				var parent = document.querySelector("#outils_edit_message_" + id + " > .btn-group:nth-last-child(2)");
				var bloc = "edit_message_" + id;

				var node = document.createElement("div");
				node.className = "btn-group groupe-boutons-barre-outils";
				node.innerHTML = "<button type='button' class='btn btn-reduit' title='Smiley A801'><img src='http://atelier801.com/favicon.ico'/></button><button class='btn btn-reduit dropdown-toggle' data-toggle='dropdown'> <span class='caret'></span></button><ul class='dropdown-menu pull-right label-message'> <table style='min-width:300px'> <tbody> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/i9Cqh.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/i9Cqh.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/51Mta.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/51Mta.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/Wbts1.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/Wbts1.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/oDd6Y.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/oDd6Y.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/so4ja.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/so4ja.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/20DUU.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/20DUU.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/lliSm.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/lliSm.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/6z7vx.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/6z7vx.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/dUgHq.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/dUgHq.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/7TTSk.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/7TTSk.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/UWRr0GJ.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/UWRr0GJ.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/8vcM6SC.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/8vcM6SC.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/1W100Wq.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/1W100Wq.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/p6AInvY.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/p6AInvY.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/aTwU9Kt.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/aTwU9Kt.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/cQh0ouT.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/cQh0ouT.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/bFuyN6p.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/bFuyN6p.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/36MbmHc.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/36MbmHc.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/xnVu4sa.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/xnVu4sa.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/m3PRUXO.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/m3PRUXO.png'/></a></li></td></tr></tbody></table></ul>";			parent.parentNode.insertBefore(node, parent.nextSibling);
				parent.parentNode.insertBefore(node, parent.nextSibling);

				node = document.createElement("div");
				node.className = "btn-group groupe-boutons-barre-outils";
				node.innerHTML = "<button type='button' class='btn btn-reduit' title='Smiley Fxie'><img src='http://i.imgur.com/EQaZwCU.png'/></button><button class='btn btn-reduit dropdown-toggle' data-toggle='dropdown'> <span class='caret'></span> </button><ul class='dropdown-menu pull-right label-message'> <table style='min-width:400px'> <tbody> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/Pp8ML.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/Pp8ML.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/QsLNX.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/QsLNX.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/HNQ3Y.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/HNQ3Y.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/qJIDs.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/qJIDs.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/Mn8jf.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/Mn8jf.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/GEW50.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/GEW50.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/MGVC4.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/MGVC4.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/oxVfm.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/oxVfm.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/Opgj5.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/Opgj5.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/SJY1r.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/SJY1r.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/DLTl5.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/DLTl5.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/mjxvy.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/mjxvy.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/obJdw.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/obJdw.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/hHOal.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/hHOal.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/lXve6.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/lXve6.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/5meym.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/5meym.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/0dXU1.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/0dXU1.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/gqvWp.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/gqvWp.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/fRe8E.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/fRe8E.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/JDqoG.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/JDqoG.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/t91LB.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/t91LB.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/WXz5q.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/WXz5q.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/uCfkP.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/uCfkP.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/61uC7.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/61uC7.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/FCJlP.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/FCJlP.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/7pEGa.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/7pEGa.png'/></a></li></td></tr></tbody></table></ul>";
				parent.parentNode.insertBefore(node, parent.nextSibling);

node = document.createElement("div");
node.className = "btn-group groupe-boutons-barre-outils";
node.innerHTML = "<button type='button' class='btn btn-reduit' title='Smileys criados por usuários'><img src='http://atelier801.com/img/icones/16/1historique-posts2.png'/></button><button class='btn btn-reduit dropdown-toggle' data-toggle='dropdown'> <span class='caret'></span> </button><ul class='dropdown-menu pull-right label-message'> <table style='min-width:400px'> <tbody> <tr> <td class='cellule-dropdown'><li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/rTgnFII.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/rTgnFII.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/Eph1x9h.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/Eph1x9h.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/W65lnia.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/W65lnia.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/xNxz3bn.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/xNxz3bn.png'/></a></li> </tr> <tr> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/ZC85E9M.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/ZC85E9M.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/T0NCaJ5.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/T0NCaJ5.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/FXjBjkM.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/FXjBjkM.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/2KiwTyJ.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/2KiwTyJ.png'/></a></li> </td> <tr></tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/X1ix6lN.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/X1ix6lN.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/1UJfPiQ.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/1UJfPiQ.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/Dzmftko.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/Dzmftko.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/5ge1vDG.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/5ge1vDG.png'/></a></li> </td> <tr> </tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/u8iGizM.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/u8iGizM.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/2ebX02S.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/2ebX02S.png'/></a></li> </td> </td></tr></tbody></table></ul>";
parent.parentNode.insertBefore(node, parent.nextSibling);

node = document.createElement("div");
node.className = "btn-group groupe-boutons-barre-outils";
node.innerHTML = "<button type='button' class='btn btn-reduit' title='Créditos'><img src='http://atelier801.com/img/pays/br.png'/></button><button class='btn btn-reduit dropdown-toggle' data-toggle='dropdown'> <span class='caret'></span> </button><ul class='dropdown-menu pull-right label-message'> <table style='min-width:400px'> <tbody> <tr> <td class='cellule-dropdown'><b>Criador</b>: Mcfloy<br><b>Tópico BR</b>: Dedavii<br><b>Smileys</b>: Melibellule, Fxie, Mrkurt, Xtayyguerleo, Doritosgotos<br><br>Atualizado 29/12 - Versão 1.0.1</td></tr></tbody></table></ul>";
parent.parentNode.insertBefore(node, parent.nextSibling);
			};
		}
})();
