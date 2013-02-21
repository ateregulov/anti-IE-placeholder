anti-IE-placeholder
===================

anti-IE-placeholder


`<script>
    $(document).ready(function () {
        /* Placeholder for IE */
        if ($.browser.msie) { // 
            $("form").find("input[type='text'], input[type='password']").each(function () {
                var tp = $(this).attr("placeholder");
                $(this).before('<p>' + tp + '</p>');
            });
        }
    });
</script>`