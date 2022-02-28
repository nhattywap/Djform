# Djform
 Django form builder
 djform builds django form templates and returns a form object

 # Usage
    from djform import *

     def make_form(class_name, attrs):
        
        try:
            fo = Global_Dict_Obj[class_name]
            return fo
        except Exception as e:
            mf = Fill_Form_Field(class_name, attrs)
            exec_obj_as_global(mf.fill())
            fo = Global_Dict_Obj[class_name]
            return fo