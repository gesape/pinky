Prereqs
-------

 - tensorflow
 - scikit-optimize
 - git clone git@github.com:HerrMuellerluedenscheid/swarming.git

Invoke
------

To start training:

    pinky --config <config_filename> --train

You can dump your examples to TFRecordDatasets to accelerate io operations:

    pinky --config <config_filename> --write <new_config_filename>

and use the newly created config file to run `--train`


Tests
-----

 - basic learning (synthetics, real data)
   # TODO: split data -> training, evaluation
 - synthetics, layered cake, train with top and bottom layer containing events.
        Validate with events within middle layer
 - evaluation using 'unknown' velocity model
 - test extrapolation with fault plane geometry
 - synthetic pretraining
 - hyperparameter optimization using skopt

Outlook
-------

 - increase z error weight -> improve z estimates
