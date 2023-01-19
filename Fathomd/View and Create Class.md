# Viewing

Like in instructorOld in /client/admin/account/code/instructor-old.coffee, just import Sessions and SessionStates as Mongo Collections from /imports/client/model/session-collections.coffee.

# Creating

Copy the code to create new DSG session (newDualSource).

Calling path for DSG session:

1. instructorOld -> newDualSource in client/sessions/games/instructor/instructor-session-config-dual-source
2. newDualSource -> DualSourceGameConfiguration from /imports/client/react-components/dual-source/instructor-config.js
3. DualSourceGameConfiguration -> DsgConfigurationForm from /imports/client/react-components/dual-source/session-config-forms.js
4. DsgConfigurationForm uses forms.js for form components -> callMeteorMethod from '/imports/client/util/react-libs/meteor-wrapper.js' w/ "createGameSession"
5. createGameSession -> platform.coffee -> Sessions, etc... in /imports/client/model/session-collections.coffee -> PlatformEventProcessor to create Session.
