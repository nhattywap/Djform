# Djform
 Django form builder
 djform builds django form templates and returns a form object

 # Usage
    from djform import forms_factory

    mf = forms_factory('LoginForm', 'field')

    pass_ = Pass_Field('Password')
    mf = forms_factory('LoginForm', ('username', pass_))