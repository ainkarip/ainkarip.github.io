<?php
/*
 * C online compiler
 * developed by Yacov Drori 18/3/2011
 * yacov@drori.org
 * http://drori.org
 *
 * for noe it is a very basic c compiler.
 * in order for this to work you need gcc to be installed on your machine.
 * description: compile the code on textbox and run it,
 * show compile errors and nice code using GeSHi project.
 *
 * liscence: GPL 2
 * todo:
 * highlght code for compilation errors
 * personalize(maybe become joomla extension);
 * generalize the paths.
 */
    session_start();
    include_once 'geshi/geshi.php';
?><!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN">
<html>
    <head>
        <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
        <title></title>
    </head>
    <body>
        <?php
        if (isset($_REQUEST['code'])){
            $newcode=stripslashes($_REQUEST['code']);
            $oName = "/var/www/ccomp/temp/" . session_id();
            $fName= $oName . ".c";
            $fHandle=fopen($fName, 'w') or die ('can\'t open file');
            fwrite($fHandle, $newcode);
            fclose($fHandle);
            //$cherro =shell_exec('chmod 777 $fName');
            $cmd = "gcc $fName -o $oName > $oName.err 2>&1";
            //echo $cmd;
            shell_exec($cmd);
            if (file_exists("$oName.err")){
                $fErr = fopen("$oName.err", "r");
                $errors = fread($fErr, filesize("$oName.err"));
            }
            $geshi=new GeSHi($newcode,'c');
            $geshi->enable_line_numbers(GESHI_FANCY_LINE_NUMBERS);
            $geshi->set_header_type(GESHI_HEADER_PRE_VALID);
        }
        ?>
        <div class="errors" name="errors"><?php echo $errors ?></div>
        <div class="codeenterd" name="codeenterd"></div><?php echo $geshi->parse_code(); ?>
        <form name="compile" action="" method="post">
            <textarea name="code"><?php echo $newcode ?></textarea><br>
            <input type="submit" name="submit" value="submit">
        </form>
    </body>
</html>
