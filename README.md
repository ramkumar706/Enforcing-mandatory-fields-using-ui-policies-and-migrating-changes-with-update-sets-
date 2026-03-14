# Enforcing-mandatory-fields-using-ui-policies-and-migrating-changes-with-update-sets-
Kabilan
onCondition() {

    if (g_form.getValue('state') == '6') {   // 6 = Resolved

        g_form.setMandatory('close_code', true);
        g_form.setMandatory('close_notes', true);

    } else {

        g_form.setMandatory('close_code', false);
        g_form.setMandatory('close_notes', false);

    }

}
