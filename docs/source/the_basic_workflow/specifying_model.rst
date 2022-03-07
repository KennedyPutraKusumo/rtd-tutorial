..  _specifying_model:
Specifying a Model
##################
You can define any Python function to specify the model for experimental design

::
    def my_function(ti_controls, tv_controls, sampling_times, model_parameters):
        return np.array([
            response1,
            response2,
        ])
The basic signature of the function is that it should take up to four input arguments
in the order given above. The argument :code:'ti_controls' is short for :emphasis:'T'ime-:emphasis:'I'nvariant
experimental controls. Likewise, :code:'tv_controls' is short for :emphasis:'T'ime-:emphasis:'V'arying Controls.

When modelling non-dynamic systems --- no time-varying and sampling times --- there
are two alternative ways to define the model function. The first is to keep

