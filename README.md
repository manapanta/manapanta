

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head id="Head1"><title>
	:: santha - Online Login Form ::
</title><link rel="stylesheet" href="../../css/bootstrap.min.css" /><link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.6.3/css/font-awesome.css" /><link rel="stylesheet" href="../../css/custom_styles.css" />
    <script src="../../Scripts/md5.js" type="text/javascript"></script>
    <style>
       
        .registrationpopup
        {
            width: 1000px;
            margin: 5px auto;
        }
        @media (max-width:1020px)
        {
            .registrationpopup
            {
                width: 90%;
            }
        }
        .registrationpopup h2
        {
            margin: 0;
            color: #A92800;
            font-size: 18px;
            margin-bottom: 5px;
            border-bottom: 1px dashed;
            padding-bottom: 3px;
        }
        .registrationpopup p
        {
            margin-bottom: 2px;
            color: #000;
            font-size: 13px;
        }
        
        .registrationpopup .inputtypestyle
        {
            width: 100%;
            margin-bottom: 3px;
            height: 30px !important;
        }
        .registrationpopup .modal-body
        {
            padding-bottom: 8px !important;
            padding-top: 10px !important;
        }
        .modal-header
        {
            padding: 6px 15px !important;
            padding-bottom: 4px !important;
        }
        .modal-footer
        {
            padding: 4px 15px !important;
        }
    </style>
    <style type="text/css">
        #flashingtext1
        {
            font-family: Trebuchet MS, sans-serif;
            font-size: 16px;
            color: blue;
            text-decoration: none;
        }
        /*Body onload popup code */
        #popup
        {
            position: absolute;
            width: 600px;
            height: 180px;
            background: #fff;
            left: 50%;
            top: 50%;
            border-radius: 5px;
            padding: 60px 0;
            margin-left: -320px; /* width/2 + padding-left */
            margin-top: -150px; /* height/2 + padding-top */
            text-align: center;
            box-shadow: 0 0 10px 0 #000;
        }
        
        #close
        {
            position: absolute;
            background: black;
            color: white;
            right: -15px;
            top: -15px;
            border-radius: 50%;
            width: 30px;
            height: 30px;
            line-height: 30px;
            text-align: center;
            font-size: 8px;
            font-weight: bold;
            font-family: 'Arial Black' , Arial, sans-serif;
            cursor: pointer;
            box-shadow: 0 0 10px 0 #000;
        }
        .body_popup
        {
            min-height: 277px;
        }
        .body_popup p
        {
            font-size: 22px;
            font-family: arial;
            color: #f00;
            padding-top: 36px;
        }
        .onload_dialog
        {
            margin-top: 90px;
        }
        
        
        .close
        {
            background: #065543;
            padding: 4px 8px;
            border-radius: 50%;
            float: right;
            margin-top: -9px;
            margin-right: -8px;
            color: #fff;
            font-weight: bold;
            text-decoration: none;
        }
        
        
        
        #mask
        {
            position: absolute;
            left: 0;
            top: 0;
            z-index: 9000;
            background-color: #000;
            display: none;
            height: 1058px !important;
        }
        #boxes .window
        {
            position: absolute;
            left: 0;
            top: 0;
            width: 664px;
            height: 464px;
            display: none;
            z-index: 9999;
            padding: 20px;
        }
        #boxes #dialog
        {
            width: 664px;
            height: auto;
            padding: 10px;
            background-color: #ffffff;
        }
        .blink_me {
                -webkit-animation-name: blinker;
                -webkit-animation-duration: 1s;
                -webkit-animation-timing-function: linear;
                -webkit-animation-iteration-count: infinite;

                -moz-animation-name: blinker;
                -moz-animation-duration: 1s;
                -moz-animation-timing-function: linear;
                -moz-animation-iteration-count: infinite;

                animation-name: blinker;
                animation-duration: 1s;
                animation-timing-function: linear;
                animation-iteration-count: infinite;
                font-size: 15px;
            }

            @-moz-keyframes blinker {  
                0% { color: red; }
            100% { color: blue; }

            }

            @-webkit-keyframes blinker {  
                0% { color: red; }
            100% { color: blue; }

            }

            @keyframes blinker {  
                0% { color: red; }
            100% { color: blue; }

            }

    </style>
    <style type="text/css">
        .close1
        {
            float: right;
            background: #00a907;
            padding: 6px;
            color: #fff !important;
            width: 30px;
            height: 30px;
            text-align: center;
            font-weight: bold;
            border-radius: 50%;
            margin-bottom: 5px;
            text-decoration: none !important;
        }
        #flashingtext
        {
            font-family: Trebuchet MS, sans-serif;
            font-size: 15px;
            color: blue;
            text-decoration: none;
        }
        #flashingtext1
        {
            font-family: Trebuchet MS, sans-serif;
            font-size: 16px;
            color: blue;
            text-decoration: none;
            text-align: justify;
        }
        
        .modal
        {
            display: block;
            background: #000000d9;
        }
        
        
        .modal-content
        {
            box-shadow: 0px 0px 3px #fdcda5;
        }
        .fade
        {
            opacity: 1;
        }
        .modal-header .close
        {
            color: #ffffff;
        }
        .modal-header
        {
            background: #ff8822;
        }
        .modal-title
        {
            margin: 0;
            line-height: 1.42857143;
            color: #fff;
            text-transform: uppercase;
            font-weight: bold;
        }
        .modal-dialog
        {
            width: 85%;
            margin: 15px auto;
        }
        .popupboxeddiv
        {
            background: #fff;
            border: 1px solid #ababab;
            border-radius: 5px;
            box-shadow: 0px 1px 4px #a29f9e;
            min-height: 120px;
            margin-bottom: 15px;
            padding: 2px;
        }
        .popupboxeddiv ol
        {
            margin: 0;
            padding: 0 28px;
            float: left;
            width: 100%;
            color: #252525;
            font-size: 13px;
        }
        .popupboxeddiv p
        {
            background: #FF9800;
            padding: 7px 15px;
            color: #fff;
            text-transform: uppercase;
            border-top-right-radius: 5px;
            border-top-left-radius: 5px;
        }
        .popupboxeddiv ol li
        {
            padding-bottom: 5px;
            border-bottom: 1px dotted #909090;
            padding-top: 5px;
        }
        .bhoechie-tab-menu a
{
text-align:left;
  padding: 23.7px 13px;
    border-bottom: 1px solid #fff !important;

}
.bhoechie-tab-menu a i {
    padding-right: 17px !important;
}
        .scrolltable {
        }
            .scrolltable p {
                color:#0635bb;
                font-size:14px;
            }
            .scrolltable table {
                width:100%;
                border-color:#000;
            }
                .scrolltable table tr:nth-child(odd) {
                    background:#f9f4db;
                }
                .scrolltable table tr:nth-child(even) {
                    background:#fff;
                }
                .scrolltable table td {
                    padding:5px 15px;
                    font-size:14px;
                }
        .rightalign {
            text-align:right;
        }
        .centeralign {
            text-align:center;
        }
        .mt0 {
    margin-top: 27px;
}
            .mt0 span {
                display:none;
            }
        .otherserviceslink {
            float: left;
    margin-left: 35%;
    background-image: linear-gradient(to right, #2e9f33 , #0082ff);
    padding: 14px 35px;
    color: #fff !important;
    border-radius: 29px;
    margin-top: 12px;
    text-transform: uppercase;
    font-weight: bold;
    box-shadow: 0px 3px 6px #807c7c;
    text-decoration: none !important;
    border:1px solid #fff;
        }
        .otherserviceslink:hover {
            
            background-image: linear-gradient(to right, #0082ff, #2e9f33);
        }
    </style>

    <script type="text/javascript">   
            
            function GetTransDetails() {

                var transId = document.getElementById("txtTransId").value;

                if (transId == "") {
                    alert("Please Enter Meeseva Application/Transaction Number");
                    return false;
                }



                if (document.getElementById('txtTransId').value != "") {

                    var LOC = document.getElementById('txtTransId').value;
                    if (LOC != "") {
                        var reg = /^[a-zA-Z]+$/;
                        var Isvalid = reg.test(LOC);
                        if (Isvalid) {
                            alert("Please Enter Valid Meeseva Application/Transaction Number");
                            document.getElementById('txtTransId').value = "";
                            document.getElementById('txtTransId').focus();
                            return false;
                        }

                        for (var i = 0; i <= (LOC.length - 1); i++) {
                            var charCode = LOC.charCodeAt(i);
                            if ((charCode >= 32 && charCode <= 47) || (charCode >= 58 && charCode <= 64) || (charCode >= 91 && charCode <= 96) || (charCode >= 123 && charCode <= 126)) {
                                alert("Please Enter Valid Meeseva Application/Transaction Number");
                                document.getElementById('txtTransId').value = "";
                                document.getElementById('txtTransId').focus();
                                return false;
                            }
                            //                        else {
                            //                            return true;
                            //                        }


                        }
                        //                                    var string = "Some string"; for (var i = 0; i < string.length; i++) { console.log(string.charCodeAt(i)); }
                    }
                }
                return true;
            }

            function GetCertDetails() {
                var applno = document.getElementById("txtApplno").value;
                if (applno == "") {
                    alert("Please Enter Meeseva Application/Transaction Number");
                    return false;
                }

                else {
                    var n = applno.length;
                    if (n >= 2) {
                        var strshortened = applno.slice(0, 2);
                        //                    if (strshortened.toUpperCase() == 'TA') {
                        //                        alert("Please enter Meeseva Application/Transaction Number");
                        //                        document.getElementById("txtApplno").value = "";
                        //                        return false;
                        //                    }
                    }
                    //window.open("CaptchaImage.aspx?Applno=" + applno + "", "", "width:1000px,height=1000px,scrollbars=1");
                }

                if (document.getElementById('txtApplno').value == "") {
                    alert("Please Enter Application/Transaction Number");
                    document.getElementById('txtApplno').focus();
                    return false;
                }
                else if (document.getElementById('txtApplno').value != "") {
                    var LOC = document.getElementById('txtApplno').value;
                    if (LOC[0] == "") {
                        alert("Empty Space is not allowed in Application/Transaction Number");
                        document.getElementById('txtApplno').focus();
                        document.getElementById('txtApplno').value = "";
                        return false;
                    }
                    if (LOC != "") {

                        var reg = /^[a-zA-Z]+$/;
                        var Isvalid = reg.test(LOC);
                        if (Isvalid) {
                            alert("Please Enter Valid Meeseva Application/Transaction Number");
                            document.getElementById('txtApplno').focus();
                            document.getElementById('txtApplno').value = "";
                            return false;
                        }
                        for (var i = 0; i <= (LOC.length - 1); i++) {
                            var charCode = LOC.charCodeAt(i);
                            if ((charCode >= 32 && charCode <= 47) || (charCode >= 58 && charCode <= 64) || (charCode >= 91 && charCode <= 96) || (charCode >= 123 && charCode <= 126)) {
                                alert("Please Enter Valid Meeseva Application/Transaction Number");
                                document.getElementById('txtApplno').value = "";
                                document.getElementById('txtApplno').focus();
                                return false;
                            }
                            //                        else {
                            //                            return true;
                            //                        }


                        }


                    }

                }
                return true;

            }


            function GetDownloadCertDetails() {
                var applno = document.getElementById("txtdownloadcer").value;
                if (applno == "") {
                    alert("Please Enter Meeseva Application/Transaction Number");
                    return false;
                }

                else {
                    var n = applno.length;
                    if (n >= 2) {
                        var strshortened = applno.slice(0, 2);
                        //                    if (strshortened.toUpperCase() == 'TA') {
                        //                        alert("Please enter Meeseva Application/Transaction Number");
                        //                        document.getElementById("txtApplno").value = "";
                        //                        return false;
                        //                    }
                    }
                    //window.open("CaptchaImage.aspx?Applno=" + applno + "", "", "width:1000px,height=1000px,scrollbars=1");
                }

                if (document.getElementById('txtdownloadcer').value == "") {
                    alert("Please Enter Application/Transaction Number");
                    document.getElementById('txtdownloadcer').focus();
                    return false;
                }
                else if (document.getElementById('txtdownloadcer').value != "") {
                    var LOC = document.getElementById('txtdownloadcer').value;
                    if (LOC[0] == "") {
                        alert("Empty Space is not allowed in Application/Transaction Number");
                        document.getElementById('txtdownloadcer').focus();
                        document.getElementById('txtdownloadcer').value = "";
                        return false;
                    }
                    if (LOC != "") {

                        var reg = /^[a-zA-Z]+$/;
                        var Isvalid = reg.test(LOC);
                        if (Isvalid) {
                            alert("Please Enter Valid Meeseva Application/Transaction Number");
                            document.getElementById('txtdownloadcer').focus();
                            document.getElementById('txtdownloadcer').value = "";
                            return false;
                        }
                        for (var i = 0; i <= (LOC.length - 1) ; i++) {
                            var charCode = LOC.charCodeAt(i);
                            if ((charCode >= 32 && charCode <= 47) || (charCode >= 58 && charCode <= 64) || (charCode >= 91 && charCode <= 96) || (charCode >= 123 && charCode <= 126)) {
                                alert("Please Enter Valid Meeseva Application/Transaction Number");
                                document.getElementById('txtdownloadcer').value = "";
                                document.getElementById('txtdownloadcer').focus();
                                return false;
                            }
                            //                        else {
                            //                            return true;
                            //                        }


                        }


                    }

                }
                return true;

            }

            function checkAlphaNumericAuthNumber() {
                var ch = String.fromCharCode(event.keyCode);
                var filter = /^[0-9a-zA-Z\/&*()-. ]/; 
                //var filter = ///^[0-9a-zA-Z\/#$%^&*()-. ]/; onkeypress="javascript:return checkAlphaNumericAuthNumber();
                if (!filter.test(ch)) {
                    event.returnValue = false;
                }
            }
            function ValidateAlphanumeric(e) {
                e = (e) ? e : event;
                var charCode = (e.charCode) ? e.charCode : ((e.keyCode) ? e.keyCode : ((e.which) ? e.which : 0));


                if ((charCode >= 32 && charCode <= 47) || (charCode >= 58 && charCode <= 64) || (charCode >= 91 && charCode <= 96) || (charCode >= 123 && charCode <= 126)) {
                    return false;
                }
                else {
                    return true;
                }

            }
            function MultipleSpaces(str) {
                var name = str.value;
                str.value = name.replace(/ +(?= )/g, '');

            }
            function lettersOnly(evt) {
                debugger;
                evt = (evt) ? evt : event;
                var charCode = (evt.charCode) ? evt.charCode : ((evt.keyCode) ? evt.keyCode :
            ((evt.which) ? evt.which : 0));
                if (charCode > 32 && (charCode < 65 || charCode > 90) &&
            (charCode < 97 || charCode > 122)) {
                    return false;
                }
                return true;
            }
        
        </script>
    <style>
        .searchrow {
              min-height: 100px;
    background: #d9efe0;
    margin: 0;
    margin-top: 10px;
    margin-bottom: 4px;
    border: 1px solid #97b4a0;
        }
        .searchrow .form-group label{
            margin-top: 13px;
    margin-bottom: 9px;
    color: #002542;
    font-size: 15px;
        }

            .searchrow .input-group {
                border: 1px solid #099853;
            }
      .searchrow .input-group  .input-group-addon {
            background: #099853;
        }

.searchrow .input-group2 {
                border: 1px solid #2f80e7;
            }
      .searchrow .input-group2  .input-group-addon {
            background: #2f80e7;
        }
      .searchrow .input-group3 {
                border: 1px solid #D28008;
            }
      .searchrow .input-group3  .input-group-addon {
            background: #D28008;
        }
        .input-group-addon input {
                background: url(../../Images/searchicon.png) !important;
                background-size: contain !important;
    background-repeat: no-repeat !important;
    height: 20px !important;
    width: 20px;
        }
        .input-group-addon {
            padding: 6px 10px;
        }
        .input-group-addon {
          
            border: 0px solid #ccc;
            border-radius: 0px;
        }
    </style>
</head>
<body>
  
    <form name="LoginForm" method="post" action="./Home.aspx" id="LoginForm">
<div>
<input type="hidden" name="__EVENTTARGET" id="__EVENTTARGET" value="" />
<input type="hidden" name="__EVENTARGUMENT" id="__EVENTARGUMENT" value="" />
<input type="hidden" name="__VIEWSTATE" id="__VIEWSTATE" value="/wEPDwULLTE2NzA2NjYyOTMPZBYCAgMPZBYCAgMPZBYCZg9kFgYCAw8WAh4Gb25ibHVyBTVqYXZhc2NyaXB0OnJldHVybiBFbmNyeXB0UGFzc3dvcmQoZXZlbnQsIDE3Njg1NTI0MjgpO2QCBw8WAh4Dc3JjBaYOZGF0YTppbWFnZS9HaWY7YmFzZTY0LFIwbEdPRGxoVUFBZUFQY0FBQUFBQUFBQU13QUFaZ0FBbVFBQXpBQUEvd0FyQUFBck13QXJaZ0FybVFBcnpBQXIvd0JWQUFCVk13QlZaZ0JWbVFCVnpBQlYvd0NBQUFDQU13Q0FaZ0NBbVFDQXpBQ0Evd0NxQUFDcU13Q3FaZ0NxbVFDcXpBQ3Evd0RWQUFEVk13RFZaZ0RWbVFEVnpBRFYvd0QvQUFEL013RC9aZ0QvbVFEL3pBRC8vek1BQURNQU16TUFaak1BbVRNQXpETUEvek1yQURNck16TXJaak1ybVRNcnpETXIvek5WQUROVk16TlZaak5WbVROVnpETlYvek9BQURPQU16T0Faak9BbVRPQXpET0Evek9xQURPcU16T3Faak9xbVRPcXpET3EvelBWQURQVk16UFZaalBWbVRQVnpEUFYvelAvQURQL016UC9aalAvbVRQL3pEUC8vMllBQUdZQU0yWUFabVlBbVdZQXpHWUEvMllyQUdZck0yWXJabVlybVdZcnpHWXIvMlpWQUdaVk0yWlZabVpWbVdaVnpHWlYvMmFBQUdhQU0yYUFabWFBbVdhQXpHYUEvMmFxQUdhcU0yYXFabWFxbVdhcXpHYXEvMmJWQUdiVk0yYlZabWJWbVdiVnpHYlYvMmIvQUdiL00yYi9abWIvbVdiL3pHYi8vNWtBQUprQU01a0FacGtBbVprQXpKa0EvNWtyQUprck01a3JacGtybVprcnpKa3IvNWxWQUpsVk01bFZacGxWbVpsVnpKbFYvNW1BQUptQU01bUFacG1BbVptQXpKbUEvNW1xQUptcU01bXFacG1xbVptcXpKbXEvNW5WQUpuVk01blZacG5WbVpuVnpKblYvNW4vQUpuL001bi9acG4vbVpuL3pKbi8vOHdBQU13QU04d0Fac3dBbWN3QXpNd0EvOHdyQU13ck04d3Jac3dybWN3cnpNd3IvOHhWQU14Vk04eFZac3hWbWN4VnpNeFYvOHlBQU15QU04eUFac3lBbWN5QXpNeUEvOHlxQU15cU04eXFac3lxbWN5cXpNeXEvOHpWQU16Vk04elZac3pWbWN6VnpNelYvOHovQU16L004ei9ac3ovbWN6L3pNei8vLzhBQVA4QU0vOEFadjhBbWY4QXpQOEEvLzhyQVA4ck0vOHJadjhybWY4cnpQOHIvLzlWQVA5Vk0vOVZadjlWbWY5VnpQOVYvLytBQVArQU0vK0FaditBbWYrQXpQK0EvLytxQVArcU0vK3FaditxbWYrcXpQK3EvLy9WQVAvVk0vL1Zadi9WbWYvVnpQL1YvLy8vQVAvL00vLy9adi8vbWYvL3pQLy8vd0FBQUFBQUFBQUFBQUFBQUNINUJBRUFBUHdBTEFBQUFBQlFBQjRBQUFqL0FDVk5Fa2h3b01HQ0NBOHFUTWh3b2NPR0VCMU8ya2V4NHI2SkZpbGl6TGpSWXNlS0h6Vm1GRGt5NU1XUit5U2hWRG1TWlVhWEZtRldsRW1SWnNxVk9FdWlOTW16NHJBWUFBQ0kyVWxVcDFHT0t4OHFoWWdqaHNBd1FpTktYZnFRWWN5Y0wwY0NZRlFSQjBhYllMRmViVmswWXlPVVp6TUtyYWhDR1VtemFPT09USXVVTE1lZ01UWXFBd29nVEVVeEFOeG1JbFl4REYrTW1ZQzZIWnZWYnVPTEJSa1paR1Q0S1lBYmt4Z0JFQWpZNlVDK053aUs4WHhES0NQSld6TlRuVXF3RWNLZHlnQllSQ043WDJDS295a3FtMFFNOEJhTlF5a0NnRmJ4dGsydUk1SFhYUjR6c2NYWWk0c2pOMUNSR0lBMEdaMFhkOXZ6S09QdklJT0sveDlQdnJ6NTgrTmppSjBwbCtORHdJeEVBemdZUTR6Qk1Dc0tWaDRvWmt0Zmc0Q3h0cHBTSG1VRTFGRFE2UlpEZFB2RTV0YyttcWdRVFUyNkFaQUpSWnA1QjFKWjRGR1lFV0FBTEVnUk1USFVKeDVGbW9nblJuUWIzUkFjWUk1WnBKeU1IRlpFVjRjM3hjZ2ViamQ0eU55R0d2cTRFRUlDU3VYYVFFSVp0TkNSa2pBNUVFTUVRWFRjZWo0VytOT0U5ZVFXWkk0WnpiampqMjhWdUtWS3k0QjRBekZoYlduU2pWL2ltQ2FZWElyNW1KczdGYWthUTA1S0V1V0FldkpKbFdRQzBhbGptRzBXV2lXUWNIWUhKNXVIRWtvUm95Y2xSMldjRlhtSjRhUW12VW1qbW1VTjZLZEFnQjZVcDBLaDJ0a2tsRTlpMmg2T21hNWFxYXB6VFNocVU2dGoxdWdvcFkxR0N1ZXNzTTVwNkVXZlNya2tRNld1Wm1leGNncnE2NjI4RG9xcnJnRUJBRHM9ZAILDw8WAh4HVmlzaWJsZWhkZBgBBR5fX0NvbnRyb2xzUmVxdWlyZVBvc3RCYWNrS2V5X18WAQUNaW1nYnRuUmVmcmVzaN6fXHhsWw03qeCM56vPL8AZZ+e4AszWNC0EXpllQ2Gc" />
</div>

<script type="text/javascript">
//<![CDATA[
var theForm = document.forms['LoginForm'];
if (!theForm) {
    theForm = document.LoginForm;
}
function __doPostBack(eventTarget, eventArgument) {
    if (!theForm.onsubmit || (theForm.onsubmit() != false)) {
        theForm.__EVENTTARGET.value = eventTarget;
        theForm.__EVENTARGUMENT.value = eventArgument;
        theForm.submit();
    }
}
//]]>
</script>


<script src="/CitizenPortal/WebResource.axd?d=XsPQCEUMdzHKgf9XbP9jrAEWUJx3YdiaqvN1zv_O4vPW8V40BLI_KX6WhheJ4AxnpgnaK6uWZO_6-_nW6UJQ5QgC6oxTm0QlvNW5C0-mxKs1&amp;t=638465256520000000" type="text/javascript"></script>


<script src="/CitizenPortal/ScriptResource.axd?d=eNfmfx1VC47Gg3F-p33K-Kb_wj8G5wjkGX9gDKGkQAGrJ-5Qn2jsfgrY_kqUiAxH6HXuvo_EQVqfuJUcHGiuQDu9u-MpNC6Q92LUFIEszGU_5ZShibQLrIGapScwcfqtHBMaq94wHiQ4HJfJ6D9U_aKVyJUUpp-pLpjQfnGZQMfP0jkbmPNNUoXz38YQmdFQ0&amp;t=2e7d0aca" type="text/javascript"></script>
<script type="text/javascript">
//<![CDATA[
if (typeof(Sys) === 'undefined') throw new Error('ASP.NET Ajax client-side framework failed to load.');
//]]>
</script>

<script src="/CitizenPortal/ScriptResource.axd?d=SNAcgrj_4mfF-tvJyG4ggnZqvpskUVvhbUvVwT4wUJyMA520MYAnJRSkdQV38-soz5OVCs9Cx6dbn0wWjcKZR8T02CvmJQMjMU-7ebKS-a335LZscknjD8RPngEYqZfhtZhgsJlXP_PDAgnV6I5sWBSXXo-gfH_cx4JKbO_DGw8Lf2jYaQ5x-zAiYpoOtTlW0&amp;t=2e7d0aca" type="text/javascript"></script>
<div>

	<input type="hidden" name="__VIEWSTATEGENERATOR" id="__VIEWSTATEGENERATOR" value="689EBCA8" />
</div>
    <script type="text/javascript">
//<![CDATA[
Sys.WebForms.PageRequestManager._initialize('ScriptManager1', 'LoginForm', ['tUPLOGIN',''], [], ['btnTGo','','btnSearch',''], 90, '');
//]]>
</script>

    <div class="container">
        <!--Body Onload Popup -->
        <!-- Modal -->
        
        <!--Body Onload Popup end -->
        <div class="top_header">
        </div>
        <div class="main_header">
            <div class="row" style="margin: 0px;">
                <img src="../../images/HRD.jpg" style="width: 100%;" />
            </div>
        </div>
        <!--Main Body start-->
        <div class="mainbody_bg">

 
            
            <div id="UPLOGIN">
	
                    <div class="row" style="padding-left: 15px; padding-right: 15px;">
                        <div class="col-lg-6 col-md-6 col-sm-6 col-xs-6 bhoechie-tab-container">
                            <div class="col-lg-5 col-md-5 col-sm-5 col-xs-5 bhoechie-tab-menu">
                                <div class="list-group">
                                    <a href="#" class="list-group-item active text-center"><i class="fa fa-user"></i><span>
                                        User Login</span> </a>
                                </div>
                                <div class="reg_bg">
                                    <div class="reg_bggreen">
                                        <a href="UnlockAccount.aspx" target="_blank" class="list-group-item text-center" style="    BACKGROUND: #1a8b55 !important;"><i
                                            class="fa fa-road"></i>Unlock User </a>
                                    </div>
                                </div>
                                <div class="reg_bg">
                                    <div class="reg_bggreen">
                                        
                                        <a href="../../UserInterface/Citizen/ForgotUserIDORPassword.aspx" target="_blank" class="list-group-item text-center"
                                            style="background-color: #125b38 !important;"><i class="fa fa-home"></i>Forgot User ID/Password
                                        </a>
                                    </div>
                                </div>
                               <div class="reg_bg">
                                    <div class="reg_bg">
                                        <a href="Registration.aspx" target="_blank" class="list-group-item text-center" style="background: #FF9B08 !important;
                                            border-radius: 0px"><i class="fa fa-pencil-square-o"></i>New Registration </a>
                                    </div>
                                </div>
                               
                               
                            </div>
                            <div class="col-lg-7 col-md-7 col-sm-7 col-xs-7 bhoechie-tab">
                                <!-- flight section -->
                                <div class="bhoechie-tab-content active" style="box-shadow:3px 4px 6px #cfcaca;">
                                    <div class="form-signin">
                                        <h2 class="form-signin-heading" style="margin-bottom: 0px !important;">
                                        </h2>
                                        <div class="col-sm-12 col-md-12" style="padding-top: 10px; padding-right: 10px;">
                                            <div style="padding: 0px;">
                                                <input name="userId" type="text" id="userId" class="form-control" placeholder="User ID" maxlength="12" />
                                                <input name="password" type="password" id="password" class="form-control" placeholder="Password" maxlength="50" onblur="javascript:return EncryptPassword(event, 1768552428);" />
                                                <input name="txtimgcode" type="text" id="txtimgcode" class="form-control" placeholder="Captcha" autocomplete="off" />
                                                <div class="row" style="position:absolute; right:18px; margin-top:-38px" >
                                                    <div class="col-sm-12">
                                                        <span style="float: left; font-size: 20px; color: #FC5A0C; text-align: center; margin-bottom: 0px;">
                                                            <img src="data:image/Gif;base64,R0lGODlhUAAeAPcAAAAAAAAAMwAAZgAAmQAAzAAA/wArAAArMwArZgArmQArzAAr/wBVAABVMwBVZgBVmQBVzABV/wCAAACAMwCAZgCAmQCAzACA/wCqAACqMwCqZgCqmQCqzACq/wDVAADVMwDVZgDVmQDVzADV/wD/AAD/MwD/ZgD/mQD/zAD//zMAADMAMzMAZjMAmTMAzDMA/zMrADMrMzMrZjMrmTMrzDMr/zNVADNVMzNVZjNVmTNVzDNV/zOAADOAMzOAZjOAmTOAzDOA/zOqADOqMzOqZjOqmTOqzDOq/zPVADPVMzPVZjPVmTPVzDPV/zP/ADP/MzP/ZjP/mTP/zDP//2YAAGYAM2YAZmYAmWYAzGYA/2YrAGYrM2YrZmYrmWYrzGYr/2ZVAGZVM2ZVZmZVmWZVzGZV/2aAAGaAM2aAZmaAmWaAzGaA/2aqAGaqM2aqZmaqmWaqzGaq/2bVAGbVM2bVZmbVmWbVzGbV/2b/AGb/M2b/Zmb/mWb/zGb//5kAAJkAM5kAZpkAmZkAzJkA/5krAJkrM5krZpkrmZkrzJkr/5lVAJlVM5lVZplVmZlVzJlV/5mAAJmAM5mAZpmAmZmAzJmA/5mqAJmqM5mqZpmqmZmqzJmq/5nVAJnVM5nVZpnVmZnVzJnV/5n/AJn/M5n/Zpn/mZn/zJn//8wAAMwAM8wAZswAmcwAzMwA/8wrAMwrM8wrZswrmcwrzMwr/8xVAMxVM8xVZsxVmcxVzMxV/8yAAMyAM8yAZsyAmcyAzMyA/8yqAMyqM8yqZsyqmcyqzMyq/8zVAMzVM8zVZszVmczVzMzV/8z/AMz/M8z/Zsz/mcz/zMz///8AAP8AM/8AZv8Amf8AzP8A//8rAP8rM/8rZv8rmf8rzP8r//9VAP9VM/9VZv9Vmf9VzP9V//+AAP+AM/+AZv+Amf+AzP+A//+qAP+qM/+qZv+qmf+qzP+q///VAP/VM//VZv/Vmf/VzP/V////AP//M///Zv//mf//zP///wAAAAAAAAAAAAAAACH5BAEAAPwALAAAAABQAB4AAAj/ACVNEkhwoMGCCA8qTMhwocOGEB1O2kex4r6JFilizLjRYseKHzVmFDky5MWR+yShVDmSZUaXFmFWlEmRZsqVOEuiNMmz4rAYAACI2UlUp1GOKx8qhYgjhsAwQiNKXfqQYcycL0cCYFQRB0abYLFebVk0YyOUZzMKrahCGUmzaOOOTIuULMegMTYqAwogTEUxANxmIlYxDF+MmYC6HZvVbuOLBRkZZGT4KYAbkxgBEAjY6UC+NwiK8XxDKCPJWzNTnUqwEcKdygBYRCN7X2CKoykqm0QM8BaNQykCgFbxtk2uI5HXXR4zscXYi4sjN1CRGIA0GZ0Xd9vzKOPvIIOK/x9Pvrz58+NjiJ0pl+NDwIxEAzgYQ4zBMCsKVh4oZktfg4CxtppSHmUE1FDQ6RZDdPvE5tc+mqgQTU26AZAJRZp5B1JZ4FGYEWAALEgRMTHUJx5FmognRnQb3RAcYI5ZpJyMHFZEV4c3xcgebjd4yNyGGvq4EEICSuXaQEIZtNCRkjA5EEMEQXTcej4W+NOE9eQWZI4Zzbjjj28VuKVKy4B4AzFhbWnSjV/imCaYXIr5mJs7FakaQ05KEuWAevJJlWQC0aljmG0WWiWQcHYHJ5uHEkoRoyclR2WcFXmJ4aQmvUmjmmUN6KdAgB6Up0Kh2tkklE9i2h6Oma5aqapzTShqU6tj1ugopY1GCuessM5p6EWfSrkkQ6WuZmexcgrq6628DoqrrgEBADs=" id="imgCaptcha" height="30" width="80" style="margin-top: -16px;" />
                                                            <input type="image" name="imgbtnRefresh" id="imgbtnRefresh" class="position-refresh" src="../../Images/CRefresh.png" style="border-width:0px;height:18px;width:20px;" />
                                                        </span>
                                                    </div>
                                                   
                                                </div>
                                                  <div class="col-sm-12" style="min-height:22px">
                                                        <p style="color: red; margin-top: 0px">
                                                            
                                                        </p>
                                                    </div>
                                                <input type="submit" name="btnsubmit" value="Sign In" onclick="return validate();" id="btnsubmit" class="btn btn-lg btn-danger btn-block" />
                                            </div>
                                        </div>
                                       
                                    </div>
                                </div>
                                <!-- train section -->
                                <!-- hotel search -->
                            </div>
                        </div>

                        <div class="col-lg-3 col-md-3 col-sm-3 col-xs-3 cm_blog" style="box-shadow:3px 4px 6px #cfcaca; border:2px solid #218f5a; padding:0px; background:#fff; text-align:center" >
                           
                           <img src="../../images/cm.png" ">
                        </div>
                         <div class="col-lg-3 col-md-3 col-sm-3 col-xs-3 cm_blog"  style="box-shadow:3px 4px 6px #cfcaca; border:2px solid #218f5a; padding:0px; background:#fff; text-align:center; border-left:0px;" >
                           
                           <img src="../../images/minister2.png" >
                        </div>

                        
                    </div>
                    

                    

                    <div class="row searchrow">
                        <div class="col-xs-12 col-sm-6">
                             <div class="form-group">
                                                <label>Check Your Application Status</label>
                                                <div class="input-group">

                                                    <input name="txtTransId" type="text" id="txtTransId" maxlength="30" autocomplete="off" class="form-control" placeholder="Enter Application/Transaction Number" aria-describedby="basic-addon2" onkeypress="javascript:return ValidateAlphanumeric(event);" />

                                                    <span class="input-group-addon" id="Span3">
                                                        <input type="submit" name="btnTGo" value="" onclick="javascript:return GetTransDetails();" id="btnTGo" class="btn" style="height: 19px; padding-left: 4px; padding-right: 4px; border-color: transparent" />
                                                    </span>

                                                </div>
                                            </div>

                                            

                                            
                        </div>


                        <div class="col-xs-12 col-sm-6">

                            <div class="form-group">
                                                <label>Preview Certificate</label>
                                                <div class="input-group input-group2">
                                                    <input name="txtApplno" type="text" id="txtApplno" maxlength="30" autocomplete="off" onkeypress="javascript:return ValidateAlphanumeric(event);" class="form-control" placeholder="Enter Application / Transaction Number" aria-describedby="basic-addon2" />
                                                    
                                                    <span class="input-group-addon" id="basic-addon2">
                                                        <input type="submit" name="btnSearch" value="" onclick="javascript:return GetCertDetails();" id="btnSearch" class="input-group-addon" style="height: 19px; padding-left: 4px; padding-right: 4px; border-color: transparent" /><i aria-hidden="true"></i></span>



                                                </div>
                                            </div>
                        </div>
                         



                    </div>
                    
                      <div class="row" style=" margin: 0px; margin-bottom: 2px; padding: 5px;
                        font-size: 14px; font-weight: bold;">
                          <div class="col-sm-12" style="padding:0px; font-size:14px; color:blue">
                           
                        
                         
                       
                        </div>
                           <div class="col-sm-12" style="padding:0px; font-size:15px; color:#000; margin-bottom:10px">
                           
                        <p style="margin-bottom:0px"><span style="color:red;">Asking Bribe? - Call ACB 1064 or send a mail to complaints-acb@ap.gov.in ఎవరైనా లంచం అడిగినా అవినీతికి పాల్పడినా టోల్ ఫ్రీ నెంబర్ 1064 కు ఫిర్యాదు చేయండి లేదా మీ ఫిర్యాదులను complaints-acb@ap.gov.in కి ఈ - మెయిల్ పంపండి.</span>  </p>
                         
                       
                        </div>
                        <div class="col-sm-12" style="padding:0px; font-size:15px; color:#000">
                           
                        <p style="margin-bottom:0px">Citizen Services Online Portal Technical Support <a href = "mailto: meeseva.support@aptonline.in" style="color:red;text-decoration: underline;cursor: pointer;">Mail ID</a>  </p>
                         
                       
                        </div>
                    </div>

                   


                   
                     



                   
                    
                    
                    <div id="dvDepts">
                    <div class="row" style="margin-top: 5px;"><div class="col-lg-3 col-sm-6"><div class="panel widget bg-green"><div class="row row-table"><div class="col-xs-4 text-center bg-green-dark pv-lg"><img src="../../images/icons/sevice_icon.png" /></div><div class="col-xs-8 pv-lg"><div class="h2 mt0"><span>23</span><a href="DeptServices.aspx??enc=6qnLLtcM2WfXFOIahFA7mA==">REVENUE DEPARTMENT</a></div></div></div></div></div><div class="col-lg-3 col-sm-6"><div class="panel widget bg-primary"><div class="row row-table"><div class="col-xs-4 text-center bg-primary-dark pv-lg"><img src="../../images/icons/sevice_icon.png" /></div><div class="col-xs-8 pv-lg"><div class="h2 mt0"><span>16</span><a href="DeptServices.aspx??enc=fMEOIocDuSSq6VBkvdjL+A==">COMMISSIONERATE OF INDUSTRIES</a></div></div></div></div></div><div class="col-lg-3 col-sm-6"><div class="panel widget bg-war"><div class="row row-table"><div class="col-xs-4 text-center bg-war-dark pv-lg"><img src="../../images/icons/sevice_icon.png" /></div><div class="col-xs-8 pv-lg"><div class="h2 mt0"><span>9</span><a href="DeptServices.aspx??enc=VThUP6n1vgIh8WUA7ZbgQA==">LEGAL METROLOGY</a></div></div></div></div></div><div class="col-lg-3 col-sm-6"><div class="panel widget bg-endo"><div class="row row-table"><div class="col-xs-4 text-center bg-endo-dark pv-lg"><img src="../../images/icons/sevice_icon.png" /></div><div class="col-xs-8 pv-lg"><div class="h2 mt0"><span>8</span><a href="DeptServices.aspx??enc=KzmFudeOOwziKb1MhBBd4g==">REGISTRATION DEPARTMENT</a></div></div></div></div></div></div><div class="row" style="margin-top: 0px;"><div class="col-lg-3 col-sm-6"><div class="panel widget bg-green"><div class="row row-table"><div class="col-xs-4 text-center bg-green-dark pv-lg"><img src="../../images/icons/sevice_icon.png" /></div><div class="col-xs-8 pv-lg"><div class="h2 mt0"><span>8</span><a href="DeptServices.aspx??enc=ZviGqiibvcX+LDNlQUWGwA==">ENDOWMENT</a></div></div></div></div></div><div class="col-lg-3 col-sm-6"><div class="panel widget bg-primary"><div class="row row-table"><div class="col-xs-4 text-center bg-primary-dark pv-lg"><img src="../../images/icons/sevice_icon.png" /></div><div class="col-xs-8 pv-lg"><div class="h2 mt0"><span>6</span><a href="DeptServices.aspx??enc=mOdbUonElWUFbfXL7JsX9w==">MINES AND GEOLOGY DEPARTMENT</a></div></div></div></div></div><div class="col-lg-3 col-sm-6"><div class="panel widget bg-war"><div class="row row-table"><div class="col-xs-4 text-center bg-war-dark pv-lg"><img src="../../images/icons/sevice_icon.png" /></div><div class="col-xs-8 pv-lg"><div class="h2 mt0"><span>4</span><a href="DeptServices.aspx??enc=Jv3rSbBMiP5VPy3QQ1Ywfg==">CDMA</a></div></div></div></div></div><div class="col-lg-3 col-sm-6"><div class="panel widget bg-endo"><div class="row row-table"><div class="col-xs-4 text-center bg-endo-dark pv-lg"><img src="../../images/icons/sevice_icon.png" /></div><div class="col-xs-8 pv-lg"><div class="h2 mt0"><span>4</span><a href="DeptServices.aspx??enc=tKOamJY+V/2omhzXMc/3NA==">DEPARTMENT OF FACTORIES</a></div></div></div></div></div></div><div class="row" style="margin-top: 0px;"><div class="col-lg-3 col-sm-6"><div class="panel widget bg-green"><div class="row row-table"><div class="col-xs-4 text-center bg-green-dark pv-lg"><img src="../../images/icons/sevice_icon.png" /></div><div class="col-xs-8 pv-lg"><div class="h2 mt0"><span>4</span><a href="DeptServices.aspx??enc=rYD3ZOnJsHgfKI45u93NfQ==">LABOUR</a></div></div></div></div></div><div class="col-lg-3 col-sm-6"><div class="panel widget bg-primary"><div class="row row-table"><div class="col-xs-4 text-center bg-primary-dark pv-lg"><img src="../../images/icons/sevice_icon.png" /></div><div class="col-xs-8 pv-lg"><div class="h2 mt0"><span>4</span><a href="DeptServices.aspx??enc=hliVrtHsDCPMLtVGm264Ig==">POLICE DEPARTMENT</a></div></div></div></div></div><div class="col-lg-3 col-sm-6"><div class="panel widget bg-war"><div class="row row-table"><div class="col-xs-4 text-center bg-war-dark pv-lg"><img src="../../images/icons/sevice_icon.png" /></div><div class="col-xs-8 pv-lg"><div class="h2 mt0"><span>1</span><a href="DeptServices.aspx??enc=LYfhFs8HH2CioN2RH3dhdw==">HEALTH DEPARTMENT</a></div></div></div></div></div><div class="col-lg-3 col-sm-6"><div class="panel widget bg-endo"><div class="row row-table"><div class="col-xs-4 text-center bg-endo-dark pv-lg"><img src="../../images/icons/sevice_icon.png" /></div><div class="col-xs-8 pv-lg"><div class="h2 mt0"><span>0</span><a href="DeptServices.aspx??enc=d6HlA6LD7NDWBCIfBUBiVQ==">EPDCL</a></div></div></div></div></div></div><div class="row" style="margin-top: 0px;"><div class="col-lg-3 col-sm-6"><div class="panel widget bg-green"><div class="row row-table"><div class="col-xs-4 text-center bg-green-dark pv-lg"><img src="../../images/icons/sevice_icon.png" /></div><div class="col-xs-8 pv-lg"><div class="h2 mt0"><span>0</span><a href="DeptServices.aspx??enc=LosVogypGbtOcyjqP7uImw==">SPDCL</a></div></div></div></div></div></div></div>
                    
                    <div class="row">
                        <div class="col-xs-12" style="text-align: right">
                            <table width="135" border="0" cellpadding="2" cellspacing="0" style="float: right;
                                border-left: 2px solid #999999;" title="Click to Verify - This site chose Symantec SSL for secure e-commerce and confidential communications.">
                                <tr>
                                    <td width="135" align="center" valign="top" style="padding-left: 9px">
                                        <script type="text/javascript" src="https://seal.websecurity.norton.com/getseal?host_name=onlineap.meeseva.gov.in&amp;size=L&amp;use_flash=NO&amp;use_transparent=Yes&amp;lang=en"></script>
                                        <br />
                                        <a href="https://www.websecurity.symantec.com/ssl-certificate" target="_blank" style="color: #000000;
                                            text-decoration: none; font: bold 10px verdana,sans-serif; letter-spacing: .5px;
                                            text-align: center; margin: 0px; padding: 0px;"></a>
                                    </td>
                                </tr>
                            </table>
                        </div>
                    </div>
                
</div>
        </div>
        <!--Main Body close -->
        <div class="footer">
            <div class="row">
                <div class="col-sm-6 footer_text">
                    <span>All Rights Reserved with Director, Electronic Services Delivery.</span>
                </div>
                <div class="col-sm-6">
                    <div class="pull-right footer_text">
                        <span>Designed & Developed by</span><img src="../../Images/APOnline-Logo.png">
                    </div>
                </div>
            </div>
        </div>
    </div>
  
    </form>
    <!-- /.modal -->
    <script type="text/javascript" src="../../js/jquery.min.js"></script>
    <script type="text/javascript" src="../../js/bootstrap.min.js"></script>
    <script type="text/javascript" src="../../js/slider.js"></script>
    <script type="text/javascript">
        //        $(document).ready(function () {
        //            $("#myModal").modal('show');
        //        });
    </script>
    <script type="text/javascript">
        $(document).ready(function () {

            $(".close").click(function () {
                $(".modal").css("display", "none");
                $(".fade").css("opacity", "0");
            });
        });
    </script>
    <script type="text/javascript">
        $(document).ready(function () {
            $("div.bhoechie-tab-menu>div.list-group>a").click(function (e) {
                e.preventDefault();
                $(this).siblings('a.active').removeClass("active");
                $(this).addClass("active");
                var index = $(this).index();
                $("div.bhoechie-tab>div.bhoechie-tab-content").removeClass("active");
                $("div.bhoechie-tab>div.bhoechie-tab-content").eq(index).addClass("active");
            });
        });


        function validate() {
            var userId = document.LoginForm.userId.value;
            if (userId == "") {
                alert("Enter your User Id.");
                document.LoginForm.userId.focus();
                return false;
            }
            //if (userId != "APOLADMIN") {
            //    alert("Enter valid User Id.");
            //    document.LoginForm.userId.focus();
            //    return false;
            //}

            for (var i = 0; i <= (userId.length - 1); i++) {
                var theChar = userId.substring(i, i + 1);
                if (!((theChar >= '0' && theChar <= '9') || (theChar >= 'a' && theChar <= 'z') || (theChar >= "A" && theChar <= "Z") || (theChar == '_') || (theChar == '.'))) {
                    alert('Enter a User Id without special characters like "' + theChar + '".');
                    document.LoginForm.userId.focus();
                    return false;
                }
            }
            if (document.LoginForm.password.value == "") {
                alert("Enter your password.")
                document.LoginForm.password.focus();
                return false;
            }
            if (document.getElementById("txtimgcode").value == "") {
                alert("Please enter Captcha");
                document.getElementById("txtimgcode").focus();
                return false;
            }
            document.getElementById('btnsubmit').value = "Signing In.. Please wait";
            return true;
        }
        var i = 1;
        function EncryptPassword(e, rno) {
            //if (i == 1) {
            if (document.getElementById('password').value != '') {
                var pwd = document.getElementById('password').value;

                var enc_pwd = MD5(MD5(pwd) + rno);
                document.getElementById('password').value = enc_pwd;
                //i = i + 1;
            }
            return true;
            //}
        }
        //For  page refresh after ideal time of 15 minutes
        var idleTime = 0;
        $(document).ready(function () {
            //Increment the idle time counter every minute.
            var idleInterval = setInterval(timerIncrement, 900000); // 15 minutes

            //Zero the idle timer on mouse movement.
            $(this).mousemove(function (e) {
                idleTime = 0;
            });
            $(this).keypress(function (e) {
                idleTime = 0;
            });
        });

        function timerIncrement() {
            idleTime = idleTime + 1;
            if (idleTime > 19) { // 20 minutes
                window.location.reload();
            }
        }
    
    </script>
    <script type="text/javascript">
        function flashtext(ele, col) {
            var tmpColCheck = document.getElementById(ele).style.color;

            if (tmpColCheck === 'blue') {
                document.getElementById(ele).style.color = col;
            } else {
                document.getElementById(ele).style.color = 'blue';
            }
        }



        setInterval(function () {
            flashtext('flashingtext1', 'red');
        }, 500); //set an interval timer up to repeat the function
    </script>
    <script type="text/javascript">
        $(document).ready(function () {
            $("#close").click(function () {
                //$("#hover").fadeOut();
                $("#popup").fadeOut();
            });

        });
    </script>
    <script type="text/javascript">
        $(window).load(function () {
            $('#myModal_bodyonload').modal('show');
        });
    </script>
    <script type="text/javascript">
        $(document).ready(function () {

            var id = '#dialog';

            //Get the screen height and width
            var maskHeight = $(document).height();
            var maskWidth = $(window).width();

            //Set heigth and width to mask to fill up the whole screen
            $('#mask').css({ 'width': maskWidth, 'height': maskHeight });

            //transition effect		
            $('#mask').fadeIn(1000);
            $('#mask').fadeTo("slow", 0.8);

            //Get the window height and width
            var winH = $(window).height();
            var winW = $(window).width();

            //Set the popup window to center
            //            $(id).css('top', winH / 2 - $(id).height() / 2);
            $(id).css('left', winW / 2 - $(id).width() / 2);

            //transition effect
            $(id).fadeIn(2000);

            //if close button is clicked
            $('.window .close1').click(function (e) {
                //Cancel the link behavior
                e.preventDefault();

                $('#mask').hide();
                $('.window').hide();
            });

            //if mask is clicked
            $('#mask').click(function () {
                $(this).hide();
                $('.window').hide();
            });

        });

    </script>
</body>
</html>
