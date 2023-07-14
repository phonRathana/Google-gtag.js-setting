# Google-gtag.js-setting
const myAPI = require('myAPI');
const isConsentGranted = require('isConsentGranted');
const addConsentListener = require('addConsentListener');

if (!isConsentGranted('ad_storage')) {
  let wasCalled = false;
  addConsentListener('ad_storage', (consentType, granted) => {
    if (wasCalled) return;
    wasCalled = true;

    const cookies = getMyCookies();
    sendFullPixel(cookies);
  });
}
{
displayName: "QP1A.190711.020 ",
name: "properties/358456605/dataStreams/4707625904/measurementProtocolSecrets/5201346021",
secretValue: "pT8SkL8HRnOYFd5T3VesPA",
},
{
adsPersonalizationEnabled: {
value: true,
},
canManageClients: true,
createTime: {
nanos: 89000000,
seconds: "1683754320",
},
creatorEmailAddress: "rathanaphon29@gmail.com",
customerId: "5362054056",
name: "properties/358456605/googleAdsLinks/5183640589",
updateTime: {
nanos: "89000000,
seconds: "1683754320",
},
eventEditData: {
name: "All.use",
parameterMutations: [
{
parameterName: "event_name",
parameterValue: "f10297db1a854b396ca2",
},
],
processingPriorityOrder: "3",
ruleTriggerConditions: [
{
comparisonType: "EQUALS",
fieldName: "event_name",
isNegated: false,
value: "100%",
},
],
streamEntityId: "4707625904",
},
parent: "properties/358456605/dataStreams/4707625904",
},
const getContainerVersion = require('getContainerVersion');
const sendPixel = require('sendPixel');

if (query('read_container_data')) {
  const cv = getContainerVersion();

  const pixelUrl = 'https://pixel.com/' +
    '?version=' + cv.version +
    '&envName=' + cv.environmentName +
    '&ctid=' + cv.containerId +
    '&debugMode=' + cv.debugMode +
    '&previewMode=' + cv.previewMo
