// ==UserScript==
// @name         Furry Project Smileys
// @namespace    https://github.com/FurryProject/Smileys
// @version      1.0
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
			node = document.createElement("div");
			node.className = "btn-group groupe-boutons-barre-outils";
			node.innerHTML = "<button type='button' class='btn btn-reduit' title='FP Smileys'><img src='http://i.imgur.com/wVkPOim.png'/></button><button class='btn btn-reduit dropdown-toggle' data-toggle='dropdown'> <span class='caret'></span></button><td class='dropdown-menu pull-right label-message'> <table style='min-width:300px'> <tbody> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/i9Cqh.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/i9Cqh.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/nfeZNUt.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/nfeZNUt.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/93XQCi5.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/93XQCi5.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/QEc9J8T.gif[/img]\", \"\", 39);'><img src='http://i.imgur.com/QEc9J8T.gif'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/YnDERRE.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/YnDERRE.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/OQF0GQM.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/OQF0GQM.png'/></a></li></td></tr></tbody></table></ul>";
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
				node.innerHTML = "<button type='button' class='btn btn-reduit' title='FP Smileys'><img src='http://atelier801.com/favicon.ico'/></button><button class='btn btn-reduit dropdown-toggle' data-toggle='dropdown'> <span class='caret'></span></button><ul class='dropdown-menu pull-right label-message'> <table style='min-width:300px'> <tbody> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/i9Cqh.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/i9Cqh.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/51Mta.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/51Mta.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/Wbts1.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/Wbts1.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/oDd6Y.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/oDd6Y.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/so4ja.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/so4ja.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/20DUU.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/20DUU.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/lliSm.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/lliSm.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/6z7vx.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/6z7vx.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/dUgHq.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/dUgHq.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/7TTSk.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/7TTSk.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/UWRr0GJ.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/UWRr0GJ.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/8vcM6SC.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/8vcM6SC.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/1W100Wq.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/1W100Wq.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/p6AInvY.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/p6AInvY.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/aTwU9Kt.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/aTwU9Kt.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/cQh0ouT.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/cQh0ouT.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/bFuyN6p.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/bFuyN6p.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/36MbmHc.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/36MbmHc.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/xnVu4sa.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/xnVu4sa.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/m3PRUXO.png[/img]\", \"\", 42);'><img src='http://i.imgur.com/m3PRUXO.png'/></a></li></td></tr></tbody></table></ul>";			parent.parentNode.insertBefore(node, parent.nextSibling);
			};
		}
})();
