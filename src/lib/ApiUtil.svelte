<script context="module" lang="ts">
  // This makes it possible to override the OpenAI API base URL in the .env file
  const apiBase = process.env.VITE_API_BASE || 'https://api.openai.com'
  const endpointCompletions = process.env.VITE_ENDPOINT_COMPLETIONS || '/v1/chat/completions'
  const endpointGenerations = process.env.VITE_ENDPOINT_GENERATIONS || '/v1/images/generations'
  const endpointModels = process.env.VITE_ENDPOINT_MODELS || '/v1/models'

  export const getApiBase = ():string => apiBase
  export const getEndpointCompletions = ():string => endpointCompletions
  export const getEndpointGenerations = ():string => endpointGenerations
  export const getEndpointModels = ():string => endpointModels
</script>
