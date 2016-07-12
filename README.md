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
			node.className = "btn-group groupe-boutons-barre-outils";
			node.innerHTML = "<button type='button' class='btn btn-reduit' title='FP Smileys'><img src='http://i.imgur.com/wVkPOim.png'/></button><button class='btn btn-reduit dropdown-toggle' data-toggle='dropdown'> <span class='caret'></span></button><ul class='dropdown-menu pull-right label-message'> <table style='min-width:300px'> <tbody> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/nfeZNUt.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/nfeZNUt.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\",  \"[img]http://i.imgur.com/93XQCi5.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/93XQCi5.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/QEc9J8T.gif[/img]\", \"\", 39);'><img src='http://i.imgur.com/QEc9J8T.gif'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/YnDERRE.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/YnDERRE.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/OQF0GQM.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/OQF0GQM.png'/></a></li></td></tr></tbody></table></ul>";			parent.parentNode.insertBefore(node, parent.nextSibling);
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
				node.innerHTML = "<button type='button' class='btn btn-reduit' title='FP Smileys'><img src='http://i.imgur.com/wVkPOim.png'/></button><button class='btn btn-reduit dropdown-toggle' data-toggle='dropdown'> <span class='caret'></span></button><ul class='dropdown-menu pull-right label-message'> <table style='min-width:300px'> <tbody> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/nfeZNUt.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/nfeZNUt.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\",  \"[img]http://i.imgur.com/93XQCi5.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/93XQCi5.png'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/QEc9J8T.gif[/img]\", \"\", 39);'><img src='http://i.imgur.com/QEc9J8T.gif'/></a></li> </td> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/YnDERRE.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/YnDERRE.png'/></a></li> </td> </tr> <tr> <td class='cellule-dropdown'> <li><a class='element-menu-outils' onclick='ajouterBBCode(\"" + bloc + "\", \"[img]http://i.imgur.com/OQF0GQM.png[/img]\", \"\", 39);'><img src='http://i.imgur.com/OQF0GQM.png'/></a></li></td></tr></tbody></table></ul>";			parent.parentNode.insertBefore(node, parent.nextSibling);
			};
		}
})();
